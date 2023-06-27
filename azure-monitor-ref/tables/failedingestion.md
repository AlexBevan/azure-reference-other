---
title: Azure Monitor Logs reference - FailedIngestion
description: Reference for FailedIngestion table in Azure Monitor Logs.
ms.topic: reference
ms.service: azure-monitor
ms.subservice: logs
ms.author: robb
author: rboucher
ms.date: 6/27/2023
---

# FailedIngestion

 Failed ingestion operations

## Categories

- Azure Resources
## Solutions

- LogManagement
## Resource types

- Azure Data Explorer Clusters




## Columns

| Column | Type | Description |
| --- | --- | --- |
| _BilledSize | real |  |
| Category | string | The category of this log |
| CorrelationId | string | The ingestion source id |
| Database | string | The name of the database holding the target table |
| Details | string | The failure's details |
| ErrorCode | string | The failure's error code |
| FailedOn | datetime | Time at which this ingest operation failed |
| FailureStatus | string | The failure's status |
| IngestionSourceId | string | A unique identifier representing the ingested source |
| IngestionSourcePath | string | The Azure blob storage URI |
| _IsBillable | string |  |
| OperationId | string | The ingestion's operation Id |
| OperationName | string | The name of this operation |
| OperationVersion | string | The version of this event |
| OriginatesFromUpdatePolicy | bool | Indicates whether or not the failure originate from an Update Policy |
| _ResourceId | string | A unique identifier for the resource that the record is associated with |
| ResultType | string | The final state of this data ingestion operation |
| RootActivityId | string | The ingestion's activity Id |
| ShouldRetry | bool | Indicates whether or not the failure is transient and should be retried |
| SourceSystem | string | The type of agent the event was collected by. For example, *OpsManager* for Windows agent, either direct connect or Operations Manager, *Linux* for all Linux agents, or *Azure* for Azure Diagnostics |
| _SubscriptionId | string | A unique identifier for the subscription that the record is associated with |
| Table | string | The name of the target table into which the data is ingested |
| TenantId | string | The Log Analytics workspace ID |
| TimeGenerated | datetime | Time at which this event is generated and logged |
| Type | string | The name of the table |
