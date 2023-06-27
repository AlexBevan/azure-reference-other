---
title: Azure Monitor Logs reference - AutoscaleEvaluationsLog
description: Reference for AutoscaleEvaluationsLog table in Azure Monitor Logs.
ms.topic: reference
ms.service: azure-monitor
ms.subservice: logs
ms.author: robb
author: rboucher
ms.date: 6/27/2023
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

| Column | Type | Description |
| --- | --- | --- |
| AutoscaleMetricName | string |  |
| AvailabilitySet | string |  |
| _BilledSize | real |  |
| Category | string |  |
| CloudServiceName | string |  |
| CloudServiceRole | string |  |
| CoolDown | int |  |
| CorrelationId | string |  |
| CurrentInstanceCount | int |  |
| DefaultInstanceCount | int |  |
| DeploymentSlot | string |  |
| EstimateScaleResult | string |  |
| EvaluationResult | string |  |
| EvaluationTime | datetime |  |
| InstanceUpdateReason | string |  |
| _IsBillable | string |  |
| LastScaleActionOperationId | string |  |
| LastScaleActionOperationStatus | string |  |
| LastScaleActionTime | datetime |  |
| MaximumInstanceCount | int |  |
| MetricData | string |  |
| MetricEndTime | datetime |  |
| MetricNamespace | string |  |
| MetricStartTime | datetime |  |
| MetricTimeGrain | string |  |
| MinimumInstanceCount | int |  |
| NewInstanceCount | int |  |
| ObservedValue | real |  |
| OperationName | string |  |
| Operator | string |  |
| Profile | string |  |
| ProfileEvaluationTime | datetime |  |
| ProfileSelected | bool |  |
| Projection | real |  |
| _ResourceId | string | A unique identifier for the resource that the record is associated with |
| ResourceId | string |  |
| ResultDescription | string |  |
| ResultType | string |  |
| SelectedAutoscaleProfile | string |  |
| ServerFarm | string |  |
| ShouldUpdateInstance | bool |  |
| SkipCurrentAutoscaleEvaluation | bool |  |
| SkipRuleEvaluationForCooldown | bool |  |
| SourceSystem | string | The type of agent the event was collected by. For example, *OpsManager* for Windows agent, either direct connect or Operations Manager, *Linux* for all Linux agents, or *Azure* for Azure Diagnostics |
| _SubscriptionId | string | A unique identifier for the subscription that the record is associated with |
| TargetResourceId | string |  |
| Threshold | real |  |
| TimeAggregationType | string |  |
| TimeGenerated | datetime |  |
| TimeGrainStatistic | string |  |
| TimeWindow | string |  |
| Type | string | The name of the table |
| Webspace | string |  |
