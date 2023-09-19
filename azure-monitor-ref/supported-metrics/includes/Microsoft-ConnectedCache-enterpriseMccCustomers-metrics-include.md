---
ms.service: azure-monitor
ms.topic: include
ms.date: 09/19/2023
ms.author: edbaynash
author: EdB-MSFT
ms.custom: Microsoft.ConnectedCache/enterpriseMccCustomers, naam
---
  
  
|Metric|Name|Unit|Aggregation|Dimensions|Time Grains|DS Export|
|---|---|---|---|---|---|---|
|Egress Mbps<p><p>Egress Throughput |`egressbps` |BitsPerSecond |Average |cachenodeid|PT1M |Yes|
|Hit Ratio<p><p>Cache hit ratio is a measurement of how many content requests a cache is able to fill successfully, compared to how many requests it receives. |`hitRatio` |Percent |Average |cachenodeid|PT1M |Yes|
|Hits<p><p>Count of hits |`hits` |Count |Count |cachenodeid|PT1M |Yes|
|Hit Mbps<p><p>Hit Throughput |`hitsbps` |BitsPerSecond |Average |cachenodeid|PT1M |Yes|
|Inbound<p><p>Inbound Throughput |`inboundbps` |BitsPerSecond |Average |cachenodeid|PT1M |Yes|
|Misses<p><p>Count of misses |`misses` |Count |Count |cachenodeid|PT1M |Yes|
|Miss Mbps<p><p>Miss Throughput |`missesbps` |BitsPerSecond |Average |cachenodeid|PT1M |Yes|
|Outbound<p><p>Outbound Throughput |`outboundbps` |BitsPerSecond |Average |cachenodeid|PT1M |Yes|