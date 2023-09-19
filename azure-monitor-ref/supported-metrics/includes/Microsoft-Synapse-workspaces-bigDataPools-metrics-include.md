---
ms.service: azure-monitor
ms.topic: include
ms.date: 09/19/2023
ms.author: edbaynash
author: EdB-MSFT
ms.custom: Microsoft.Synapse/workspaces/bigDataPools, naam
---
  
  
|Metric|Name|Unit|Aggregation|Dimensions|Time Grains|DS Export|
|---|---|---|---|---|---|---|
|vCores allocated<p><p>Allocated vCores for an Apache Spark Pool |`BigDataPoolAllocatedCores` |Count |Maximum, Minimum, Average, Total |SubmitterId|PT1M |No|
|Memory allocated (GB)<p><p>Allocated Memory for Apach Spark Pool (GB) |`BigDataPoolAllocatedMemory` |Count |Maximum, Minimum, Average, Total |SubmitterId|PT1M |No|
|Active Apache Spark applications<p><p>Total Active Apache Spark Pool Applications |`BigDataPoolApplicationsActive` |Count |Maximum, Minimum, Average |JobState|PT1M |No|
|Ended Apache Spark applications<p><p>Count of Apache Spark pool applications ended |`BigDataPoolApplicationsEnded` |Count |Total |JobType, JobResult|PT1M |No|