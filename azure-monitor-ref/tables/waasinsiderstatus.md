---
title: Azure Monitor Logs reference - WaaSInsiderStatus
description: Reference for WaaSInsiderStatus table in Azure Monitor Logs.
ms.topic: reference
ms.service: azure-monitor
ms.subservice: logs
ms.author: robb
author: rboucher
ms.date: 6/27/2023
---

# WaaSInsiderStatus

 Summary of each run of your update schedule with details like how many updates were not installed etc.

## Categories

- Desktop Analytics
## Solutions

- Update Compliance




## Columns

| Column | Type | Description |
| --- | --- | --- |
| _BilledSize | real |  |
| Computer | string |  |
| ComputerID | string |  |
| _IsBillable | string |  |
| LastScan | datetime |  |
| OSArchitecture | string |  |
| OSBuild | string |  |
| OSEdition | string |  |
| OSFamily | string |  |
| OSName | string |  |
| OSRevisionNumber | int |  |
| OSVersion | string |  |
| SourceSystem | string | The type of agent the event was collected by. For example, *OpsManager* for Windows agent, either direct connect or Operations Manager, *Linux* for all Linux agents, or *Azure* for Azure Diagnostics |
| TimeGenerated | datetime |  |
| Type | string | The name of the table |
