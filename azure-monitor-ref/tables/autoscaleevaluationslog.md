---
title: Azure Monitor Logs reference - AutoscaleEvaluationsLog
description: Reference for AutoscaleEvaluationsLog table in Azure Monitor Logs.
ms.topic: reference
ms.service: azure-monitor
ms.subservice: logs
ms.author: bwren
author: bwren
ms.date: 8/5/2021
---

# AutoscaleEvaluationsLog

 

## Categories

- Azure Monitor
- Virtual Machines
- Azure Resources
## Solutions

- LogManagement
## Resource types

- Azure Monitor autoscale settings




## Columns

|Column|Type|Description|
|---|---|---|
|AutoscaleMetricName|string||
|AvailabilitySet|string||
|Category|string||
|CloudServiceName|string||
|CloudServiceRole|string||
|CoolDown|int||
|CorrelationId|string||
|CurrentInstanceCount|int||
|DefaultInstanceCount|int||
|DeploymentSlot|string||
|EstimateScaleResult|string||
|EvaluationResult|string||
|EvaluationTime|datetime||
|InstanceUpdateReason|string||
|LastScaleActionOperationId|string||
|LastScaleActionOperationStatus|string||
|LastScaleActionTime|datetime||
|MaximumInstanceCount|int||
|MetricData|string||
|MetricEndTime|datetime||
|MetricNamespace|string||
|MetricStartTime|datetime||
|MetricTimeGrain|string||
|MinimumInstanceCount|int||
|NewInstanceCount|int||
|ObservedValue|real||
|OperationName|string||
|Operator|string||
|Profile|string||
|ProfileEvaluationTime|datetime||
|ProfileSelected|bool||
|Projection|real||
|ResourceId|string||
|ResultDescription|string||
|ResultType|string||
|SelectedAutoscaleProfile|string||
|ServerFarm|string||
|ShouldUpdateInstance|bool||
|SkipCurrentAutoscaleEvaluation|bool||
|SkipRuleEvaluationForCooldown|bool||
|SourceSystem|string||
|TargetResourceId|string||
|Threshold|real||
|TimeAggregationType|string||
|TimeGenerated|datetime||
|TimeGrainStatistic|string||
|TimeWindow|string||
|Type|string|The name of the table|
|Webspace|string||
