---
ms.service: azure-monitor
ms.topic: include
ms.date: 09/19/2023
ms.author: edbaynash
author: EdB-MSFT
ms.custom: Microsoft.Logic/IntegrationServiceEnvironments, naam
---
  
  
|Metric|Name|Unit|Aggregation|Dimensions|Time Grains|DS Export|
|---|---|---|---|---|---|---|
|Action Latency <p><p>Latency of completed workflow actions. |`ActionLatency` |Seconds |Average |No Dimensions|PT1M |Yes|
|Actions Completed <p><p>Number of workflow actions completed. |`ActionsCompleted` |Count |Total |No Dimensions|PT1M |Yes|
|Actions Failed <p><p>Number of workflow actions failed. |`ActionsFailed` |Count |Total |No Dimensions|PT1M |Yes|
|Actions Skipped <p><p>Number of workflow actions skipped. |`ActionsSkipped` |Count |Total |No Dimensions|PT1M |Yes|
|Actions Started <p><p>Number of workflow actions started. |`ActionsStarted` |Count |Total |No Dimensions|PT1M |Yes|
|Actions Succeeded <p><p>Number of workflow actions succeeded. |`ActionsSucceeded` |Count |Total |No Dimensions|PT1M |Yes|
|Action Success Latency <p><p>Latency of succeeded workflow actions. |`ActionSuccessLatency` |Seconds |Average |No Dimensions|PT1M |Yes|
|Connector Memory Usage for Integration Service Environment<p><p>Connector memory usage for integration service environment. |`IntegrationServiceEnvironmentConnectorMemoryUsage` |Percent |Average |No Dimensions|PT1M |Yes|
|Connector Processor Usage for Integration Service Environment<p><p>Connector processor usage for integration service environment. |`IntegrationServiceEnvironmentConnectorProcessorUsage` |Percent |Average |No Dimensions|PT1M |Yes|
|Workflow Memory Usage for Integration Service Environment<p><p>Workflow memory usage for integration service environment. |`IntegrationServiceEnvironmentWorkflowMemoryUsage` |Percent |Average |No Dimensions|PT1M |Yes|
|Workflow Processor Usage for Integration Service Environment<p><p>Workflow processor usage for integration service environment. |`IntegrationServiceEnvironmentWorkflowProcessorUsage` |Percent |Average |No Dimensions|PT1M |Yes|
|Run Latency<p><p>Latency of completed workflow runs. |`RunLatency` |Seconds |Average |No Dimensions|PT1M |Yes|
|Runs Cancelled<p><p>Number of workflow runs cancelled. |`RunsCancelled` |Count |Total |No Dimensions|PT1M |Yes|
|Runs Completed<p><p>Number of workflow runs completed. |`RunsCompleted` |Count |Total |No Dimensions|PT1M |Yes|
|Runs Failed<p><p>Number of workflow runs failed. |`RunsFailed` |Count |Total |No Dimensions|PT1M |Yes|
|Runs Started<p><p>Number of workflow runs started. |`RunsStarted` |Count |Total |No Dimensions|PT1M |Yes|
|Runs Succeeded<p><p>Number of workflow runs succeeded. |`RunsSucceeded` |Count |Total |No Dimensions|PT1M |Yes|
|Run Success Latency<p><p>Latency of succeeded workflow runs. |`RunSuccessLatency` |Seconds |Average |No Dimensions|PT1M |Yes|
|Trigger Fire Latency <p><p>Latency of fired workflow triggers. |`TriggerFireLatency` |Seconds |Average |No Dimensions|PT1M |Yes|
|Trigger Latency <p><p>Latency of completed workflow triggers. |`TriggerLatency` |Seconds |Average |No Dimensions|PT1M |Yes|
|Triggers Completed <p><p>Number of workflow triggers completed. |`TriggersCompleted` |Count |Total |No Dimensions|PT1M |Yes|
|Triggers Failed <p><p>Number of workflow triggers failed. |`TriggersFailed` |Count |Total |No Dimensions|PT1M |Yes|
|Triggers Fired <p><p>Number of workflow triggers fired. |`TriggersFired` |Count |Total |No Dimensions|PT1M |Yes|
|Triggers Skipped<p><p>Number of workflow triggers skipped. |`TriggersSkipped` |Count |Total |No Dimensions|PT1M |Yes|
|Triggers Started <p><p>Number of workflow triggers started. |`TriggersStarted` |Count |Total |No Dimensions|PT1M |Yes|
|Triggers Succeeded <p><p>Number of workflow triggers succeeded. |`TriggersSucceeded` |Count |Total |No Dimensions|PT1M |Yes|
|Trigger Success Latency <p><p>Latency of succeeded workflow triggers. |`TriggerSuccessLatency` |Seconds |Average |No Dimensions|PT1M |Yes|