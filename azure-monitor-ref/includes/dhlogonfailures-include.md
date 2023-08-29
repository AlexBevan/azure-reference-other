---
ms.service: azure-monitor
ms.topic: include
ms.date: 08/28/2023
ms.author: edbaynash
author: EdB-MSFT
ms.custom: DHLogonFailures
---


| Column | Type | Description |
|---|---|---|
| _BilledSize | real | The record size in bytes |
| Computer | string |   |
| ComputerID | string |   |
| Country | string |   |
| _IsBillable | string | Specifies whether ingesting the data is billable. When _IsBillable is `false` ingestion isn't billed to your Azure account |
| LogonStatus | string |   |
| LogonSubStatus | string |   |
| Manufacturer | string |   |
| Model | string |   |
| ModelFamily | string |   |
| OSArchitecture | string |   |
| OSBuildNumber | int |   |
| OSEdition | string |   |
| OSRevisionNumber | int |   |
| OSVersion | string |   |
| ProviderId | string |   |
| ProviderName | string |   |
| SignInFailureCount | long |   |
| SignInFailureReason | string |   |
| SignInUserError | string |   |
| SuggestedSignInRemediation | string |   |
| TimeGenerated | datetime |   |
| Type | string | The name of the table |
