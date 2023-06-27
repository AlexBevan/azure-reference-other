---
title: Azure Monitor Logs reference - DeviceAppCrash
description: Reference for DeviceAppCrash table in Azure Monitor Logs.
ms.topic: reference
ms.service: azure-monitor
ms.subservice: logs
ms.author: robb
author: rboucher
ms.date: 6/27/2023
---

# DeviceAppCrash

 

## Categories

- Workloads
## Solutions

- Surface Hub




## Columns

| Column | Type | Description |
| --- | --- | --- |
| AppID | string |  |
| _BilledSize | real |  |
| Computer | string |  |
| EventId | int |  |
| EventName | string |  |
| HealthServiceId | string |  |
| _IsBillable | string |  |
| ProviderId | string |  |
| SourceSystem | string | The type of agent the event was collected by. For example, *OpsManager* for Windows agent, either direct connect or Operations Manager, *Linux* for all Linux agents, or *Azure* for Azure Diagnostics |
| TimeGenerated | datetime |  |
| Type | string | The name of the table |
