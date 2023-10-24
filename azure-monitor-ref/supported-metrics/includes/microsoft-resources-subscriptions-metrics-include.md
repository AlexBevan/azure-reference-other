---
ms.service: azure-monitor
ms.topic: include
ms.date: 10/18/2023
ms.author: edbaynash
author: EdB-MSFT
ms.custom: microsoft.resources/subscriptions, naam
---
<!--
NOTE:  This content is automatically generated using API calls to Azure. 
Any edits made on these files will be overwritten in the next run of the script. 
There is no benefit in editing these files directly.  
-->
  
  
|Metric|Name in REST API|Unit|Aggregation|Dimensions|Time Grains|DS Export|
|---|---|---|---|---|---|---|
|**Latency**<p><p>Latency data for all requests to Azure Resource Manager |`Latency` |Seconds |Average |`IsCustomerOriginated`, `Method`, `Namespace`, `RequestRegion`, `ResourceType`, `StatusCode`, `StatusCodeClass`, `Microsoft.SubscriptionId`|PT1M |No|
|**Traffic**<p><p>Traffic data for all requests to Azure Resource Manager |`Traffic` |Count |Count |`IsCustomerOriginated`, `Method`, `Namespace`, `RequestRegion`, `ResourceType`, `StatusCode`, `StatusCodeClass`, `Microsoft.SubscriptionId`|PT1M |No|