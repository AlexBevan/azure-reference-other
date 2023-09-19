---
ms.service: azure-monitor
ms.topic: include
ms.date: 09/19/2023
ms.author: edbaynash
author: EdB-MSFT
ms.custom: microsoft.hybridnetwork/networkfunctions, naam
---
  
  
|Metric|Name|Unit|Aggregation|Dimensions|Time Grains|DS Export|
|---|---|---|---|---|---|---|
|Average CPU Utilization<p><p>Total average percentage of virtual CPU utilization at one minute interval. The total number of virtual CPU is based on user configured value in SKU definition. Further filter can be applied based on RoleName defined in SKU. |`HyperVVirtualProcessorUtilization` |Percent |Average, Maximum, Minimum |InstanceName|PT1M |Yes|