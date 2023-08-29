---
ms.service: azure-monitor
ms.topic: include
ms.date: 08/28/2023
ms.author: edbaynash
author: EdB-MSFT
ms.custom: WDAVThreat
---


| Column | Type | Description |
|---|---|---|
| _BilledSize | real | The record size in bytes |
| Computer | string |   |
| ComputerID | string |   |
| _IsBillable | string | Specifies whether ingesting the data is billable. When _IsBillable is `false` ingestion isn't billed to your Azure account |
| IsCloudSignature | bool |   |
| LastScan | datetime |   |
| MoreInformation | string |   |
| RemediationAction | string |   |
| SourceSystem | string | The type of agent the event was collected by. For example, `OpsManager` for Windows agent, either direct connect or Operations Manager, `Linux` for all Linux agents, or `Azure` for Azure Diagnostics |
| ThreatAction | string |   |
| ThreatAlertLevel | string |   |
| ThreatCategory | string |   |
| ThreatEncyclopediaLink | string |   |
| ThreatError | string |   |
| ThreatFamily | string |   |
| ThreatId | int |   |
| ThreatName | string |   |
| ThreatReportId | string |   |
| ThreatStatus | string |   |
| TimeGenerated | datetime |   |
| Type | string | The name of the table |
