---
ms.service: azure-monitor
ms.topic: include
ms.date: 09/19/2023
ms.author: edbaynash
author: EdB-MSFT
ms.custom: Microsoft.Synapse/workspaces, naam
---
  
  
|Metric|Name|Unit|Aggregation|Dimensions|Time Grains|DS Export|
|---|---|---|---|---|---|---|
|Data processed (bytes)<p><p>Amount of data processed by queries |`BuiltinSqlPoolDataProcessedBytes` |Bytes |Total |No Dimensions|PT1M |No|
|Login attempts<p><p>Count of login attempts that succeded or failed |`BuiltinSqlPoolLoginAttempts` |Count |Average, Minimum, Maximum, Total |Result|PT1M |No|
|Requests ended<p><p>Count of Requests that succeeded, failed, or were cancelled |`BuiltinSqlPoolRequestsEnded` |Count |Average, Minimum, Maximum, Total |Result|PT1M |No|
|Activity runs ended<p><p>Count of integration activities that succeeded, failed, or were cancelled |`IntegrationActivityRunsEnded` |Count |Count, Total |Result, FailureType, Activity, ActivityType, Pipeline|PT1M, PT1H |No|
|Link connection events<p><p>Number of Synapse Link connection events including start, stop and failure. |`IntegrationLinkConnectionEvents` |Count |Total |EventType, LinkConnectionName|PT1M |No|
|Link processed rows<p><p>Changed row count processed by Synapse Link. |`IntegrationLinkProcessedChangedRows` |Count |Total |TableName, LinkConnectionName|PT1M |No|
|Link processed data volume (bytes)<p><p>Data volume in bytes processed by Synapse Link. |`IntegrationLinkProcessedDataVolume` |Bytes |Total |TableName, LinkTableStatus, LinkConnectionName|PT1M |No|
|Link latency in seconds<p><p>Synapse Link data processing latency in seconds. |`IntegrationLinkProcessingLatencyInSeconds` |Count |Maximum, Minimum, Average |LinkConnectionName|PT1M |No|
|Link table events<p><p>Number of Synapse Link table events including snapshot, removal and failure. |`IntegrationLinkTableEvents` |Count |Total |TableName, EventType, LinkConnectionName|PT1M |No|
|Pipeline runs ended<p><p>Count of integration pipeline runs that succeeded, failed, or were cancelled |`IntegrationPipelineRunsEnded` |Count |Count, Total |Result, FailureType, Pipeline|PT1M, PT1H |No|
|Trigger Runs ended<p><p>Count of integration triggers that succeeded, failed, or were cancelled |`IntegrationTriggerRunsEnded` |Count |Count, Total |Result, FailureType, Trigger|PT1M, PT1H |No|
|Backlogged input events (preview)<p><p>This is a preview metric available in East US, West Europe. Number of input events sources backlogged. |`SQLStreamingBackloggedInputEventSources` |Count |Total |SQLPoolName, SQLDatabaseName, JobName, LogicalName, PartitionId, ProcessorInstance|PT1M |No|
|Data conversion errors (preview)<p><p>This is a preview metric available in East US, West Europe. Number of output events that could not be converted to the expected output schema. Error policy can be changed to 'Drop' to drop events that encounter this scenario. |`SQLStreamingConversionErrors` |Count |Total |SQLPoolName, SQLDatabaseName, JobName, LogicalName, PartitionId, ProcessorInstance|PT1M |No|
|Input deserialization errors (preview)<p><p>This is a preview metric available in East US, West Europe. Number of input events that could not be deserialized. |`SQLStreamingDeserializationError` |Count |Total |SQLPoolName, SQLDatabaseName, JobName, LogicalName, PartitionId, ProcessorInstance|PT1M |No|
|Early input events (preview)<p><p>This is a preview metric available in East US, West Europe. Number of input events which application time is considered early compared to arrival time, according to early arrival policy. |`SQLStreamingEarlyInputEvents` |Count |Total |SQLPoolName, SQLDatabaseName, JobName, LogicalName, PartitionId, ProcessorInstance|PT1M |No|
|Input event bytes (preview)<p><p>This is a preview metric available in East US, West Europe. Amount of data received by the streaming job, in bytes. This can be used to validate that events are being sent to the input source. |`SQLStreamingInputEventBytes` |Count |Total |SQLPoolName, SQLDatabaseName, JobName, LogicalName, PartitionId, ProcessorInstance|PT1M |No|
|Input events (preview)<p><p>This is a preview metric available in East US, West Europe. Number of input events. |`SQLStreamingInputEvents` |Count |Total |SQLPoolName, SQLDatabaseName, JobName, LogicalName, PartitionId, ProcessorInstance|PT1M |No|
|Input sources received (preview)<p><p>This is a preview metric available in East US, West Europe. Number of input events sources per second. |`SQLStreamingInputEventsSourcesPerSecond` |Count |Total |SQLPoolName, SQLDatabaseName, JobName, LogicalName, PartitionId, ProcessorInstance|PT1M |No|
|Late input events (preview)<p><p>This is a preview metric available in East US, West Europe. Number of input events which application time is considered late compared to arrival time, according to late arrival policy. |`SQLStreamingLateInputEvents` |Count |Total |SQLPoolName, SQLDatabaseName, JobName, LogicalName, PartitionId, ProcessorInstance|PT1M |No|
|Out of order events (preview)<p><p>This is a preview metric available in East US, West Europe. Number of Event Hub Events (serialized messages) received by the Event Hub Input Adapter, received out of order that were either dropped or given an adjusted timestamp, based on the Event Ordering Policy. |`SQLStreamingOutOfOrderEvents` |Count |Total |SQLPoolName, SQLDatabaseName, JobName, LogicalName, PartitionId, ProcessorInstance|PT1M |No|
|Output events (preview)<p><p>This is a preview metric available in East US, West Europe. Number of output events. |`SQLStreamingOutputEvents` |Count |Total |SQLPoolName, SQLDatabaseName, JobName, LogicalName, PartitionId, ProcessorInstance|PT1M |No|
|Watermark delay (preview)<p><p>This is a preview metric available in East US, West Europe. Output watermark delay in seconds. |`SQLStreamingOutputWatermarkDelaySeconds` |Count |Maximum, Minimum, Average |SQLPoolName, SQLDatabaseName, JobName, LogicalName, PartitionId, ProcessorInstance|PT1M |No|
|Resource % utilization (preview)<p><p>This is a preview metric available in East US, West Europe. Resource utilization expressed as a percentage. High utilization indicates that the job is using close to the maximum allocated resources. |`SQLStreamingResourceUtilization` |Percent |Maximum, Minimum, Average |SQLPoolName, SQLDatabaseName, JobName, LogicalName, PartitionId, ProcessorInstance|PT1M |No|
|Runtime errors (preview)<p><p>This is a preview metric available in East US, West Europe. Total number of errors related to query processing (excluding errors found while ingesting events or outputting results). |`SQLStreamingRuntimeErrors` |Count |Total |SQLPoolName, SQLDatabaseName, JobName, LogicalName, PartitionId, ProcessorInstance|PT1M |No|