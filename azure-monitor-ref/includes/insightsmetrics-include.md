---
ms.service: azure-monitor
ms.topic: include
ms.date: 08/28/2023
ms.author: edbaynash
author: EdB-MSFT
ms.custom: InsightsMetrics
---


| Column | Type | Description |
|---|---|---|
| AgentId | string |   |
| _BilledSize | real | The record size in bytes |
| Computer | string |   |
| _IsBillable | string | Specifies whether ingesting the data is billable. When _IsBillable is `false` ingestion isn't billed to your Azure account |
| Name | string |   |
| Namespace | string |   |
| Origin | string |   |
| _ResourceId | string | A unique identifier for the resource that the record is associated with |
| SourceSystem | string | The type of agent the event was collected by. For example, `OpsManager` for Windows agent, either direct connect or Operations Manager, `Linux` for all Linux agents, or `Azure` for Azure Diagnostics |
| _SubscriptionId | string | A unique identifier for the subscription that the record is associated with |
| Tags | string |   |
| TimeGenerated | datetime |   |
| Type | string | The name of the table |
| Val | real |   |
| Value | string |   |
