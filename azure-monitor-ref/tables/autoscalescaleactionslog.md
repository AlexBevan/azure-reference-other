---
title: Azure Monitor Logs reference - AutoscaleScaleActionsLog
description: Reference for AutoscaleScaleActionsLog table in Azure Monitor Logs.
ms.topic: reference
ms.service: azure-monitor
ms.subservice: logs
ms.author: bwren
author: bwren
ms.date: 9/17/2020
---

# AutoscaleScaleActionsLog

 

## Categories

- Azure Resources
- Virtual Machines
- Azure Monitor
## Solutions

- LogManagement
## Resource types

- Azure Monitor autoscale settings




## Columns

|Column|Type|Description|
|---|---|---|
|Category|string||
|CorrelationId|string||
|CreatedAsyncScaleActionJob|bool||
|CreatedAsyncScaleActionJobId|string||
|CurrentInstanceCount|int||
|NewInstanceCount|int||
|OperationName|string||
|ResourceId|string||
|ResultDescription|string||
|ResultType|string||
|ScaleActionMessage|string||
|ScaleActionOperationId|string||
|ScaleActionOperationStatus|string||
|ScaleDirection|string||
|SourceSystem|string||
|TargetResourceId|string||
|TimeGenerated|datetime||
|Type|string|The name of the table|
