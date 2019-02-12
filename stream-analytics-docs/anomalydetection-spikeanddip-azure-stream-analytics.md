---
title: "AnomalyDetection_SpikeAndDip (Azure Stream Analytics) | Microsoft Docs"
description: ""
applies_to: 
  - "Azure"
services: stream-analytics
author: mamccrea
ms.service: stream-analytics
ms.topic: reference
ms.assetid: 
ms.workload: data-services
ms.date: 02/12/2018
ms.author: mamccrea
---

# AnomalyDetection_SpikeAndDip (Azure Stream Analytics) (Preview)

Temporary anomalies in a time series event stream are known as spikes and dips. These anomalies are detected in Azure Stream Analytics using the Machine Learning based **AnomalyDetection_SpikeAndDip** operator. The underlying ML model uses the adaptive kernel density estimation algorithm.

## Syntax

```SQL
AnomalyDetection_SpikeAndDip(
    <scalar_expression>,
    <confidence>,
    <historySize>,
    <mode>)
OVER ([PARTITION BY <partition key>]
    LIMIT DURATION(<unit>, <length>)
    [WHEN boolean_expression])
```

## Arguments

**scalar_expression**

Event column or computed field over which the model performs anomaly detection. Allowed values for this parameter include FLOAT or BIGINT data types that return a single (scalar) value.

The wildcard expression (*) is not allowed. Also, *scalar_expression* cannot contain other analytic functions or external functions.

**confidence**

A percentage number from 1.00 to 100 (inclusive) that sets the sensitivity of the ML model. Lower the confidence, higher could be the number of anomalies detected, and vice versa. Users are advised to start from an arbitrary number between 90 and 100 and adjust this based on the results observed in dev/test.

**historySize**

The number of events in a sliding window that the model continuously learns from and uses for scoring the next event for anomalousness. Typically, this should represent the period of time of normal behavior to enable the model to flag a subsequent anomaly. Users are advised to start with an educated guess using historical logs, and adjust it based on the results observed in dev/test.

**mode**

A string parameter whose value is “spikes”, “dips”, or “spikesanddips”, to detect only spikes, only dips, or both spikes and dips, respectively.

**OVER ( [ partition_by_clause ] limit_duration_clause [when_clause])**

**partition_by_clause**

Users may want to partition a model’s training based on a particular column in the events. For example, if several sensors with different sensor IDs are feeding into the same Stream Analytics job, partitioning by sensor ID trains a different ML model for each sensor as every sensor’s behavior patterns may be slightly different. 

The model applies the same function parameter settings across all the partitions.

**limit_duration_clause** DURATION(<unit>, <length>)

This is the size of the sliding window within Stream Analytics in terms of time. We recommend setting the size of this time window to be equal to the time it takes to generate historySize number of events in steady state. The maximum supported value is 7 days (as with all other Stream Analytics windows and durations).

**when_clause**

Specifies boolean condition for the events to be accepted by the model to perform anomaly detection. The *when_clause* is optional.

## Return Types

The function returns a nested record composed of the following columns:

**IsAnomaly**

A BIGINT (0 or 1) indicating if the event was anomalous or not.

**Score**

The computed p-value score (float) indicating how anomalous an event is. Lower scores mean a lower probability that the event is part of the same distribution, and hence the more anomalous it is.

## Examples

Basic example, assuming a uniform input rate of 1 event per second in a 2 minute sliding window with a history size of 120 events. The final SELECT statement extracts and outputs the score and anomaly status with a confidence level of 95%.

```SQL
WITH AnomalyDetectionStep AS
(
    SELECT
        EVENTENQUEUEDUTCTIME aASs time,
        CAST(temperature AS FLOAT) as temp,
        AnomalyDetection_SpikeAndDip(CAST(temperature AS FLOAT), 95, 120, 'spikesanddips')
        OVER(LIMIT DURATION(second, 120)) AS SpikeAndDipScores
    FROM input
)
SELECT
    time,
    temp,
    CAST(GetRecordPropertyValue(SpikeAndDipScores, 'Score') as FLOAT) AS
    SpikeAndDipScore,
    CAST(GetRecordPropertyValue(SpikeAndDipScores, 'IsAnomaly') AS BIGINT) AS
    IsSpikeAndDipAnomaly
INTO output
FROM AnomalyDetectionStep
```

Example with a non-uniform input stream that is made uniform using a tumbling window of 1 second:

```SQL
WITH SmootheningStep AS
(
    SELECT
        System.Timestamp as time,
        AVG(CAST(temperature as float)) as temp
    FROM input
    GROUP BY TUMBLINGWINDOW(second, 1)
),
AnomalyDetectionStep AS
(
    SELECT
    time,
    temp,
    AnomalyDetection_SpikeAndDip(temp, 95, 120, 'spikesanddips') 
        OVER(LIMIT DURATION(second, 120)) as SpikeAndDipScores
    FROM SmootheningStep
)
SELECT
    time,
    temp,
    CAST(GetRecordPropertyValue(SpikeAndDipScores, 'Score') AS FLOAT) As
    SpikeAndDipScore,
    CAST(GetRecordPropertyValue(SpikeAndDipScores, 'IsAnomaly') AS BIGINT) AS
    IsSpikeAndDipAnomaly
INTO output
FROM AnomalyDetectionStep
```

Example with a partitioned query to train a separate model per sensor:

```SQL
WITH AnomalyDetectionStep AS
(
    SELECT
        sensorid,
        System.Timestamp AS time,
        CAST(temperature AS FLOAT) AS temp,
        AnomalyDetection_SpikeAndDip(CAST(temperature AS FLOAT), 95, 120, 'spikesanddips')
            OVER(PARTITION BY sensorid LIMIT DURATION(second, 120)) AS SpikeAndDipScores
    FROM input
)
SELECT
    CAST (sensorid AS NVARCHAR(max)) AS sensoridstring,
    time,
    temp,
    CAST(GetRecordPropertyValue(SpikeAndDipScores, 'Score') as float) AS
    SpikeAndDipScore,
    CAST(GetRecordPropertyValue(SpikeAndDipScores, 'IsAnomaly') AS BIGINT) AS
    IsSpikeAndDipAnomaly
INTO output
FROM AnomalyDetectionStep
```