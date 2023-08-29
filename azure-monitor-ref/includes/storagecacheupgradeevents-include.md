---
ms.service: azure-monitor
ms.topic: include
ms.date: 08/28/2023
ms.author: edbaynash
author: EdB-MSFT
ms.custom: StorageCacheUpgradeEvents
---


| Column | Type | Description |
|---|---|---|
| AvailableFirmwareVersion | string | The firmware version for upgrade, if available. |
| _BilledSize | real | The record size in bytes |
| CorrelationId | string | Unique identifier to be used to correlate logs, if available. |
| CurrentFirmwareVersion | string | The firmware version currently running. |
| Description | string | The description of the upgrade event. |
| _IsBillable | string | Specifies whether ingesting the data is billable. When _IsBillable is `false` ingestion isn't billed to your Azure account |
| Location | string | The region of the resource associated with the event. |
| _ResourceId | string | A unique identifier for the resource that the record is associated with |
| SourceSystem | string | The type of agent the event was collected by. For example, `OpsManager` for Windows agent, either direct connect or Operations Manager, `Linux` for all Linux agents, or `Azure` for Azure Diagnostics |
| _SubscriptionId | string | A unique identifier for the subscription that the record is associated with |
| TenantId | string | The Log Analytics workspace ID |
| TimeGenerated | datetime | Timestamp (UTC) when the log was created. |
| Type | string | The name of the table |
