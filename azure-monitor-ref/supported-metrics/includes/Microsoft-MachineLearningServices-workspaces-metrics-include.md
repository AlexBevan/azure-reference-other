---
ms.service: azure-monitor
ms.topic: include
ms.date: 09/19/2023
ms.author: edbaynash
author: EdB-MSFT
ms.custom: Microsoft.MachineLearningServices/workspaces, arm
---
  
  
|Metric|Name|Unit|Aggregation|Dimensions|Time Grains|DS Export|
|---|---|---|---|---|---|---|
|Active Cores<p><p>Number of active cores |`Active Cores` |Count |Average, Maximum, Minimum, Total |Scenario, ClusterName|PT1M |Yes|
|Active Nodes<p><p>Number of Acitve nodes. These are the nodes which are actively running a job. |`Active Nodes` |Count |Average, Maximum, Minimum, Total |Scenario, ClusterName|PT1M |Yes|
|Cancel Requested Runs<p><p>Number of runs where cancel was requested for this workspace. Count is updated when cancellation request has been received for a run. |`Cancel Requested Runs` |Count |Total, Average, Minimum, Maximum, Count |Scenario, RunType, PublishedPipelineId, ComputeType, PipelineStepType, ExperimentName|PT1M |Yes|
|Cancelled Runs<p><p>Number of runs cancelled for this workspace. Count is updated when a run is successfully cancelled. |`Cancelled Runs` |Count |Total, Average, Minimum, Maximum, Count |Scenario, RunType, PublishedPipelineId, ComputeType, PipelineStepType, ExperimentName|PT1M |Yes|
|Completed Runs<p><p>Number of runs completed successfully for this workspace. Count is updated when a run has completed and output has been collected. |`Completed Runs` |Count |Total, Average, Minimum, Maximum, Count |Scenario, RunType, PublishedPipelineId, ComputeType, PipelineStepType, ExperimentName|PT1M |Yes|
|CpuCapacityMillicores<p><p>Maximum capacity of a CPU node in millicores. Capacity is aggregated in one minute intervals. |`CpuCapacityMillicores` |Count |Average, Maximum, Minimum, Total |RunId, InstanceId, ComputeName|PT1M |Yes|
|CpuMemoryCapacityMegabytes<p><p>Maximum memory utilization of a CPU node in megabytes. Utilization is aggregated in one minute intervals. |`CpuMemoryCapacityMegabytes` |Count |Average, Maximum, Minimum, Total |RunId, InstanceId, ComputeName|PT1M |Yes|
|CpuMemoryUtilizationMegabytes<p><p>Memory utilization of a CPU node in megabytes. Utilization is aggregated in one minute intervals. |`CpuMemoryUtilizationMegabytes` |Count |Average, Maximum, Minimum, Total |RunId, InstanceId, ComputeName|PT1M |Yes|
|CpuMemoryUtilizationPercentage<p><p>Memory utilization percentage of a CPU node. Utilization is aggregated in one minute intervals. |`CpuMemoryUtilizationPercentage` |Count |Average, Maximum, Minimum, Total |RunId, InstanceId, ComputeName|PT1M |Yes|
|CpuUtilization<p><p>Percentage of utilization on a CPU node. Utilization is reported at one minute intervals. |`CpuUtilization` |Count |Average, Maximum, Minimum, Total |Scenario, runId, NodeId, ClusterName|PT1M |Yes|
|CpuUtilizationMillicores<p><p>Utilization of a CPU node in millicores. Utilization is aggregated in one minute intervals. |`CpuUtilizationMillicores` |Count |Average, Maximum, Minimum, Total |RunId, InstanceId, ComputeName|PT1M |Yes|
|CpuUtilizationPercentage<p><p>Utilization percentage of a CPU node. Utilization is aggregated in one minute intervals. |`CpuUtilizationPercentage` |Count |Average, Maximum, Minimum, Total |RunId, InstanceId, ComputeName|PT1M |Yes|
|DiskAvailMegabytes<p><p>Available disk space in megabytes. Metrics are aggregated in one minute intervals. |`DiskAvailMegabytes` |Count |Average, Maximum, Minimum, Total |RunId, InstanceId, ComputeName|PT1M |Yes|
|DiskReadMegabytes<p><p>Data read from disk in megabytes. Metrics are aggregated in one minute intervals. |`DiskReadMegabytes` |Count |Average, Maximum, Minimum, Total |RunId, InstanceId, ComputeName|PT1M |Yes|
|DiskUsedMegabytes<p><p>Used disk space in megabytes. Metrics are aggregated in one minute intervals. |`DiskUsedMegabytes` |Count |Average, Maximum, Minimum, Total |RunId, InstanceId, ComputeName|PT1M |Yes|
|DiskWriteMegabytes<p><p>Data written into disk in megabytes. Metrics are aggregated in one minute intervals. |`DiskWriteMegabytes` |Count |Average, Maximum, Minimum, Total |RunId, InstanceId, ComputeName|PT1M |Yes|
|Errors<p><p>Number of run errors in this workspace. Count is updated whenever run encounters an error. |`Errors` |Count |Total, Average, Minimum, Maximum, Count |Scenario|PT1M |Yes|
|Failed Runs<p><p>Number of runs failed for this workspace. Count is updated when a run fails. |`Failed Runs` |Count |Total, Average, Minimum, Maximum, Count |Scenario, RunType, PublishedPipelineId, ComputeType, PipelineStepType, ExperimentName|PT1M |Yes|
|Finalizing Runs<p><p>Number of runs entered finalizing state for this workspace. Count is updated when a run has completed but output collection still in progress. |`Finalizing Runs` |Count |Total, Average, Minimum, Maximum, Count |Scenario, RunType, PublishedPipelineId, ComputeType, PipelineStepType, ExperimentName|PT1M |Yes|
|GpuCapacityMilliGPUs<p><p>Maximum capacity of a GPU device in milli-GPUs. Capacity is aggregated in one minute intervals. |`GpuCapacityMilliGPUs` |Count |Average, Maximum, Minimum, Total |RunId, InstanceId, DeviceId, ComputeName|PT1M |Yes|
|GpuEnergyJoules<p><p>Interval energy in Joules on a GPU node. Energy is reported at one minute intervals. |`GpuEnergyJoules` |Count |Average, Maximum, Minimum, Total |Scenario, runId, rootRunId, InstanceId, DeviceId, ComputeName|PT1M |Yes|
|GpuMemoryCapacityMegabytes<p><p>Maximum memory capacity of a GPU device in megabytes. Capacity aggregated in at one minute intervals. |`GpuMemoryCapacityMegabytes` |Count |Average, Maximum, Minimum, Total |RunId, InstanceId, DeviceId, ComputeName|PT1M |Yes|
|GpuMemoryUtilization<p><p>Percentage of memory utilization on a GPU node. Utilization is reported at one minute intervals. |`GpuMemoryUtilization` |Count |Average, Maximum, Minimum, Total |Scenario, runId, NodeId, DeviceId, ClusterName|PT1M |Yes|
|GpuMemoryUtilizationMegabytes<p><p>Memory utilization of a GPU device in megabytes. Utilization aggregated in at one minute intervals. |`GpuMemoryUtilizationMegabytes` |Count |Average, Maximum, Minimum, Total |RunId, InstanceId, DeviceId, ComputeName|PT1M |Yes|
|GpuMemoryUtilizationPercentage<p><p>Memory utilization percentage of a GPU device. Utilization aggregated in at one minute intervals. |`GpuMemoryUtilizationPercentage` |Count |Average, Maximum, Minimum, Total |RunId, InstanceId, DeviceId, ComputeName|PT1M |Yes|
|GpuUtilization<p><p>Percentage of utilization on a GPU node. Utilization is reported at one minute intervals. |`GpuUtilization` |Count |Average, Maximum, Minimum, Total |Scenario, runId, NodeId, DeviceId, ClusterName|PT1M |Yes|
|GpuUtilizationMilliGPUs<p><p>Utilization of a GPU device in milli-GPUs. Utilization is aggregated in one minute intervals. |`GpuUtilizationMilliGPUs` |Count |Average, Maximum, Minimum, Total |RunId, InstanceId, DeviceId, ComputeName|PT1M |Yes|
|GpuUtilizationPercentage<p><p>Utilization percentage of a GPU device. Utilization is aggregated in one minute intervals. |`GpuUtilizationPercentage` |Count |Average, Maximum, Minimum, Total |RunId, InstanceId, DeviceId, ComputeName|PT1M |Yes|
|IBReceiveMegabytes<p><p>Network data received over InfiniBand in megabytes. Metrics are aggregated in one minute intervals. |`IBReceiveMegabytes` |Count |Average, Maximum, Minimum, Total |RunId, InstanceId, ComputeName, DeviceId|PT1M |Yes|
|IBTransmitMegabytes<p><p>Network data sent over InfiniBand in megabytes. Metrics are aggregated in one minute intervals. |`IBTransmitMegabytes` |Count |Average, Maximum, Minimum, Total |RunId, InstanceId, ComputeName, DeviceId|PT1M |Yes|
|Idle Cores<p><p>Number of idle cores |`Idle Cores` |Count |Average, Maximum, Minimum, Total |Scenario, ClusterName|PT1M |Yes|
|Idle Nodes<p><p>Number of idle nodes. Idle nodes are the nodes which are not running any jobs but can accept new job if available. |`Idle Nodes` |Count |Average, Maximum, Minimum, Total |Scenario, ClusterName|PT1M |Yes|
|Leaving Cores<p><p>Number of leaving cores |`Leaving Cores` |Count |Average, Maximum, Minimum, Total |Scenario, ClusterName|PT1M |Yes|
|Leaving Nodes<p><p>Number of leaving nodes. Leaving nodes are the nodes which just finished processing a job and will go to Idle state. |`Leaving Nodes` |Count |Average, Maximum, Minimum, Total |Scenario, ClusterName|PT1M |Yes|
|Model Deploy Failed<p><p>Number of model deployments that failed in this workspace |`Model Deploy Failed` |Count |Total, Average, Minimum, Maximum, Count |Scenario, StatusCode|PT1M |Yes|
|Model Deploy Started<p><p>Number of model deployments started in this workspace |`Model Deploy Started` |Count |Total, Average, Minimum, Maximum, Count |Scenario|PT1M |Yes|
|Model Deploy Succeeded<p><p>Number of model deployments that succeeded in this workspace |`Model Deploy Succeeded` |Count |Total, Average, Minimum, Maximum, Count |Scenario|PT1M |Yes|
|Model Register Failed<p><p>Number of model registrations that failed in this workspace |`Model Register Failed` |Count |Total, Average, Minimum, Maximum, Count |Scenario, StatusCode|PT1M |Yes|
|Model Register Succeeded<p><p>Number of model registrations that succeeded in this workspace |`Model Register Succeeded` |Count |Total, Average, Minimum, Maximum, Count |Scenario|PT1M |Yes|
|NetworkInputMegabytes<p><p>Network data received in megabytes. Metrics are aggregated in one minute intervals. |`NetworkInputMegabytes` |Count |Average, Maximum, Minimum, Total |RunId, InstanceId, ComputeName, DeviceId|PT1M |Yes|
|NetworkOutputMegabytes<p><p>Network data sent in megabytes. Metrics are aggregated in one minute intervals. |`NetworkOutputMegabytes` |Count |Average, Maximum, Minimum, Total |RunId, InstanceId, ComputeName, DeviceId|PT1M |Yes|
|Not Responding Runs<p><p>Number of runs not responding for this workspace. Count is updated when a run enters Not Responding state. |`Not Responding Runs` |Count |Total, Average, Minimum, Maximum, Count |Scenario, RunType, PublishedPipelineId, ComputeType, PipelineStepType, ExperimentName|PT1M |Yes|
|Not Started Runs<p><p>Number of runs in Not Started state for this workspace. Count is updated when a request is received to create a run but run information has not yet been populated.  |`Not Started Runs` |Count |Total, Average, Minimum, Maximum, Count |Scenario, RunType, PublishedPipelineId, ComputeType, PipelineStepType, ExperimentName|PT1M |Yes|
|Preempted Cores<p><p>Number of preempted cores |`Preempted Cores` |Count |Average, Maximum, Minimum, Total |Scenario, ClusterName|PT1M |Yes|
|Preempted Nodes<p><p>Number of preempted nodes. These nodes are the low priority nodes which are taken away from the available node pool. |`Preempted Nodes` |Count |Average, Maximum, Minimum, Total |Scenario, ClusterName|PT1M |Yes|
|Preparing Runs<p><p>Number of runs that are preparing for this workspace. Count is updated when a run enters Preparing state while the run environment is being prepared. |`Preparing Runs` |Count |Total, Average, Minimum, Maximum, Count |Scenario, RunType, PublishedPipelineId, ComputeType, PipelineStepType, ExperimentName|PT1M |Yes|
|Provisioning Runs<p><p>Number of runs that are provisioning for this workspace. Count is updated when a run is waiting on compute target creation or provisioning. |`Provisioning Runs` |Count |Total, Average, Minimum, Maximum, Count |Scenario, RunType, PublishedPipelineId, ComputeType, PipelineStepType, ExperimentName|PT1M |Yes|
|Queued Runs<p><p>Number of runs that are queued for this workspace. Count is updated when a run is queued in compute target. Can occure when waiting for required compute nodes to be ready. |`Queued Runs` |Count |Total, Average, Minimum, Maximum, Count |Scenario, RunType, PublishedPipelineId, ComputeType, PipelineStepType, ExperimentName|PT1M |Yes|
|Quota Utilization Percentage<p><p>Percent of quota utilized |`Quota Utilization Percentage` |Count |Average, Maximum, Minimum, Total |Scenario, ClusterName, VmFamilyName, VmPriority|PT1M |Yes|
|Started Runs<p><p>Number of runs running for this workspace. Count is updated when run starts running on required resources. |`Started Runs` |Count |Total, Average, Minimum, Maximum, Count |Scenario, RunType, PublishedPipelineId, ComputeType, PipelineStepType, ExperimentName|PT1M |Yes|
|Starting Runs<p><p>Number of runs started for this workspace. Count is updated after request to create run and run info, such as the Run Id, has been populated |`Starting Runs` |Count |Total, Average, Minimum, Maximum, Count |Scenario, RunType, PublishedPipelineId, ComputeType, PipelineStepType, ExperimentName|PT1M |Yes|
|StorageAPIFailureCount<p><p>Azure Blob Storage API calls failure count. |`StorageAPIFailureCount` |Count |Average, Maximum, Minimum, Total |RunId, InstanceId, ComputeName|PT1M |Yes|
|StorageAPISuccessCount<p><p>Azure Blob Storage API calls success count. |`StorageAPISuccessCount` |Count |Average, Maximum, Minimum, Total |RunId, InstanceId, ComputeName|PT1M |Yes|
|Total Cores<p><p>Number of total cores |`Total Cores` |Count |Average, Maximum, Minimum, Total |Scenario, ClusterName|PT1M |Yes|
|Total Nodes<p><p>Number of total nodes. This total includes some of Active Nodes, Idle Nodes, Unusable Nodes, Premepted Nodes, Leaving Nodes |`Total Nodes` |Count |Average, Maximum, Minimum, Total |Scenario, ClusterName|PT1M |Yes|
|Unusable Cores<p><p>Number of unusable cores |`Unusable Cores` |Count |Average, Maximum, Minimum, Total |Scenario, ClusterName|PT1M |Yes|
|Unusable Nodes<p><p>Number of unusable nodes. Unusable nodes are not functional due to some unresolvable issue. Azure will recycle these nodes. |`Unusable Nodes` |Count |Average, Maximum, Minimum, Total |Scenario, ClusterName|PT1M |Yes|
|Warnings<p><p>Number of run warnings in this workspace. Count is updated whenever a run encounters a warning. |`Warnings` |Count |Total, Average, Minimum, Maximum, Count |Scenario|PT1M |Yes|