---
ms.service: azure-monitor
ms.topic: include
ms.date: 09/19/2023
ms.author: edbaynash
author: EdB-MSFT
ms.custom: Microsoft.Cloudtest/hostedpools, naam
---
  
  
|Metric|Name|Unit|Aggregation|Dimensions|Time Grains|DS Export|
|---|---|---|---|---|---|---|
|Allocated<p><p>Resources that are allocated |`Allocated` |Count |Average, Maximum, Minimum |PoolId, SKU, Images, ProviderName|PT1M |Yes|
|AllocationDurationMs<p><p>Average time to allocate requests (ms) |`AllocationDurationMs` |Milliseconds |Average |PoolId, Type, ResourceRequestType, Image|PT1M |Yes|
|Count<p><p>Number of requests in last dump |`Count` |Count |Count |RequestType, Status, PoolId, Type, ErrorCode, FailureStage|PT1M |Yes|
|NotReady<p><p>Resources that are not ready to be used |`NotReady` |Count |Average, Maximum, Minimum |PoolId, SKU, Images, ProviderName|PT1M |Yes|
|PendingReimage<p><p>Resources that are pending reimage |`PendingReimage` |Count |Average, Maximum, Minimum |PoolId, SKU, Images, ProviderName|PT1M |Yes|
|PendingReturn<p><p>Resources that are pending return |`PendingReturn` |Count |Average, Maximum, Minimum |PoolId, SKU, Images, ProviderName|PT1M |Yes|
|Provisioned<p><p>Resources that are provisioned |`Provisioned` |Count |Average, Maximum, Minimum |PoolId, SKU, Images, ProviderName|PT1M |Yes|
|Ready<p><p>Resources that are ready to be used |`Ready` |Count |Average, Maximum, Minimum |PoolId, SKU, Images, ProviderName|PT1M |Yes|
|Starting<p><p>Resources that are starting |`Starting` |Count |Average, Maximum, Minimum |PoolId, SKU, Images, ProviderName|PT1M |Yes|
|Total<p><p>Total Number of Resources |`Total` |Count |Average, Maximum, Minimum |PoolId, SKU, Images, ProviderName|PT1M |Yes|