---
ms.service: azure-monitor
ms.topic: include
ms.date: 08/28/2023
ms.author: edbaynash
author: EdB-MSFT
ms.custom: UAComputer
---


| Column | Type | Description |
|---|---|---|
| AppIssues | int |   |
| _BilledSize | real | The record size in bytes |
| Computer | string |   |
| ComputerID | string |   |
| ConfigMgrClientID | string |   |
| DeploymentError | string |   |
| DeploymentErrorDetails | string |   |
| DeploymentStatus | string |   |
| DriverIssues | int |   |
| HoursToUninstall | int |   |
| InventoryVersion | string |   |
| _IsBillable | string | Specifies whether ingesting the data is billable. When _IsBillable is `false` ingestion isn't billed to your Azure account |
| ItemRank | int |   |
| LastScan | datetime |   |
| Manufacturer | string |   |
| Model | string |   |
| OriginBuild | string |   |
| OriginOSVersion | string |   |
| OSArchitecture | string |   |
| OSBuild | string |   |
| OSEdition | string |   |
| OSVersion | string |   |
| SourceSystem | string | The type of agent the event was collected by. For example, `OpsManager` for Windows agent, either direct connect or Operations Manager, `Linux` for all Linux agents, or `Azure` for Azure Diagnostics |
| SysReqIssues | int |   |
| TargetBuild | string |   |
| TargetOSVersion | string |   |
| TimeGenerated | datetime |   |
| TotalIssues | int |   |
| Type | string | The name of the table |
| UninstallComment | string |   |
| UninstallReason | string |   |
| UpgradeAssessment | string |   |
| UpgradeDecision | string |   |
| UserAction | string |   |
