---
title: Azure Monitor Logs reference - DeviceConnectSession
description: Reference for DeviceConnectSession table in Azure Monitor Logs.
ms.topic: reference
ms.service: azure-monitor
ms.subservice: logs
ms.author: robb
author: rboucher
ms.date: 6/15/2023
---

# DeviceConnectSession

 

## Categories

- Workloads
## Solutions

- Surface Hub




## Columns

| Column | Type | Description |
| --- | --- | --- |
| _BilledSize | real |  |
| Computer | string |  |
| DeviceType | string |  |
| EventId | int |  |
| EventName | string |  |
| HealthServiceId | string |  |
| _IsBillable | string |  |
| Opcode | int |  |
| ProviderId | string |  |
| SerialNumber | string |  |
| sessionClass | string |  |
| sessionConnected | bool |  |
| sessionDurationMilliSeconds | real |  |
| sessionType | string |  |
| SourceSystem | string | The type of agent the event was collected by. For example, *OpsManager* for Windows agent, either direct connect or Operations Manager, *Linux* for all Linux agents, or *Azure* for Azure Diagnostics |
| TimeGenerated | datetime |  |
| Type | string | The name of the table |
| wasCleanShutdown | bool |  |
