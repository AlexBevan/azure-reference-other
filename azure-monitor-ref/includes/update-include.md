---
ms.service: azure-monitor
ms.topic: include
ms.date: 08/28/2023
ms.author: edbaynash
author: EdB-MSFT
ms.custom: Update
---


| Column | Type | Description |
|---|---|---|
| ApprovalSource | string |   |
| Approved | bool |   |
| _BilledSize | real | The record size in bytes |
| BulletinID | string |   |
| BulletinUrl | string |   |
| Classification | string |   |
| Computer | string |   |
| ComputerEnvironment | string |   |
| CVENumbers | string |   |
| InstallTimeAvailable | bool |   |
| InstallTimeDeviationRangeSeconds | real |   |
| InstallTimePredictionSeconds | real |   |
| _IsBillable | string | Specifies whether ingesting the data is billable. When _IsBillable is `false` ingestion isn't billed to your Azure account |
| KBID | string |   |
| ManagementGroupName | string |   |
| MSRCBulletinID | string |   |
| MSRCSeverity | string |   |
| Optional | bool |   |
| OSFullName | string |   |
| OSName | string |   |
| OSType | string |   |
| OSVersion | string |   |
| PackageRepository | string |   |
| PackageSeverity | string |   |
| Product | string |   |
| ProductArch | string |   |
| ProductVersion | string |   |
| PublishedDate | datetime |   |
| RebootBehavior | string |   |
| Resource | string |   |
| ResourceGroup | string |   |
| ResourceId | string |   |
| _ResourceId | string | A unique identifier for the resource that the record is associated with |
| ResourceProvider | string |   |
| ResourceType | string |   |
| RevisionNumber | string |   |
| SourceComputerId | string |   |
| SourceSystem | string | The type of agent the event was collected by. For example, `OpsManager` for Windows agent, either direct connect or Operations Manager, `Linux` for all Linux agents, or `Azure` for Azure Diagnostics |
| SubscriptionId | string |   |
| _SubscriptionId | string | A unique identifier for the subscription that the record is associated with |
| TimeGenerated | datetime |   |
| Title | string |   |
| Type | string | The name of the table |
| UpdateID | string |   |
| UpdateState | string |   |
| VMUUID | string |   |
