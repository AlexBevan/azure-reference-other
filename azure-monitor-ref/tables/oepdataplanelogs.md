---
title: Azure Monitor Logs reference - OEPDataplaneLogs
description: Reference for OEPDataplaneLogs table in Azure Monitor Logs.
ms.topic: reference
ms.service: azure-monitor
ms.subservice: logs
ms.author: edbaynash
author: EdB-MSFT
ms.date: 7/10/2023
---

# OEPDataplaneLogs

 Contains logs for HTTP requests & responses for the Indexer Service API, in OSDU Data Platform, and Microsoft Energy Data Services. The Indexer service, indexes the metadata store to support search. The indexer service will automatically take items that are newly added to storage and index the attributes from the schema associated with the kind attribute.

## Categories

- Azure Resources
## Solutions

- LogManagement
## Resource types

- Azure Data Manager for Energy




## Columns

| Column | Type | Description |
| --- | --- | --- |
| _BilledSize | real | The record size in bytes |
| Category | string | Logs generated as a result of operations executed using OAK APIs are grouped into categories. Categories in OAK are logical groupings based on the data source. |
| CorrelationId | string | Unique identifier to be used to correlate logs, when available. |
| _IsBillable | string | Specifies whether ingesting the data is billable. When _IsBillable is *false* ingestion isn't billed to your Azure account |
| Location | string | The region of the resource emitting the event. |
| LogLevel | string | Log level of message (INFO, WARN, ERROR, etc.). |
| Message | string | Log details as a result of operation performed. |
| OperationName | string | The operation name for which the log entry was created. |
| _ResourceId | string | A unique identifier for the resource that the record is associated with |
| SourceSystem | string | The type of agent the event was collected by. For example, *OpsManager* for Windows agent, either direct connect or Operations Manager, *Linux* for all Linux agents, or *Azure* for Azure Diagnostics |
| _SubscriptionId | string | A unique identifier for the subscription that the record is associated with |
| TenantId | string | The Log Analytics workspace ID |
| TimeGenerated | datetime | Timestamp (UTC) when the log was created. |
| Type | string | The name of the table |