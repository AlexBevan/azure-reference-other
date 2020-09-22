---
title: Azure Monitor Logs reference - HDInsightStormLogs
description: Reference for HDInsightStormLogs table in Azure Monitor Logs.
ms.topic: reference
ms.service: azure-monitor
ms.subservice: logs
ms.author: bwren
author: bwren
ms.date: 9/17/2020
---

# HDInsightStormLogs

 All Logs from Storm cluster nodes.

## Categories

- Azure Resources
## Solutions

- LogManagement
## Resource types

- HDInsight Clusters




## Columns

|Column|Type|Description|
|---|---|---|
|ClusterName|string|Name of cluster.|
|CorrelationId|string|The ID for correlated events. Can be used to identify correlated events between multiple tables.|
|HostName|string|Name of host where log was emitted.|
|LogType|string|The name of the log file that a record came from (e.g. StormNimbus, StormSupervisor).|
|Message|string|message from Storm log.|
|OperationName|string|The operation associated with log record.|
|_ResourceId|string|A unique identifier for the resource that the record is associated with|
|SourceSystem|string||
|TenantId|string||
|TimeGenerated|datetime|The timestamp (UTC) of when the log was generated.|
|Type|string|The name of the table|
