---
title: Azure Monitor Logs reference - ETWEvent
description: Reference for ETWEvent table in Azure Monitor Logs.
ms.topic: reference
ms.service: azure-monitor
ms.subservice: logs
ms.author: robb
author: rboucher
ms.date: 6/29/2023
---

# ETWEvent

 

## Categories

- Virtual Machines
## Solutions

- LogManagement




## Columns

| Column | Type | Description |
| --- | --- | --- |
| AzureDeploymentID | string |  |
| _BilledSize | real |  |
| ChannelName | string |  |
| Computer | string |  |
| EventId | int |  |
| EventMessage | string |  |
| EventSourceName | string |  |
| _IsBillable | string |  |
| KeywordName | string |  |
| Level | string |  |
| Message | string |  |
| OpcodeName | string |  |
| Pid | int |  |
| ProviderGuid | string |  |
| Role | string |  |
| SourceSystem | string | The type of agent the event was collected by. For example, *OpsManager* for Windows agent, either direct connect or Operations Manager, *Linux* for all Linux agents, or *Azure* for Azure Diagnostics |
| TaskName | string |  |
| Tid | int |  |
| TimeGenerated | datetime |  |
| Type | string | The name of the table |
