---
ms.service: azure-monitor
ms.topic: include
ms.date: 09/19/2023
ms.author: edbaynash
author: EdB-MSFT
ms.custom: Microsoft.Storage/storageAccounts/queueServices, naam
---
  
  
|Metric|Name|Unit|Aggregation|Dimensions|Time Grains|DS Export|
|---|---|---|---|---|---|---|
|Availability<p><p>The percentage of availability for the storage service or the specified API operation. Availability is calculated by taking the TotalBillableRequests value and dividing it by the number of applicable requests, including those that produced unexpected errors. All unexpected errors result in reduced availability for the storage service or the specified API operation. |`Availability` |Percent |Average, Minimum, Maximum |GeoType, ApiName, Authentication|PT1M |Yes|
|Egress<p><p>The amount of egress data. This number includes egress to external client from Azure Storage as well as egress within Azure. As a result, this number does not reflect billable egress. |`Egress` |Bytes |Total, Average, Minimum, Maximum |GeoType, ApiName, Authentication|PT1M |Yes|
|Ingress<p><p>The amount of ingress data, in bytes. This number includes ingress from an external client into Azure Storage as well as ingress within Azure. |`Ingress` |Bytes |Total, Average, Minimum, Maximum |GeoType, ApiName, Authentication|PT1M |Yes|
|Queue Capacity<p><p>The amount of Queue storage used by the storage account. |`QueueCapacity` |Bytes |Average |No Dimensions|PT1H |Yes|
|Queue Count<p><p>The number of queues in the storage account. |`QueueCount` |Count |Average |No Dimensions|PT1H |Yes|
|Queue Message Count<p><p>The number of unexpired queue messages in the storage account. |`QueueMessageCount` |Count |Average |No Dimensions|PT1H |Yes|
|Success E2E Latency<p><p>The average end-to-end latency of successful requests made to a storage service or the specified API operation, in milliseconds. This value includes the required processing time within Azure Storage to read the request, send the response, and receive acknowledgment of the response. |`SuccessE2ELatency` |MilliSeconds |Average, Minimum, Maximum |GeoType, ApiName, Authentication|PT1M |Yes|
|Success Server Latency<p><p>The average time used to process a successful request by Azure Storage. This value does not include the network latency specified in SuccessE2ELatency. |`SuccessServerLatency` |MilliSeconds |Average, Minimum, Maximum |GeoType, ApiName, Authentication|PT1M |Yes|
|Transactions<p><p>The number of requests made to a storage service or the specified API operation. This number includes successful and failed requests, as well as requests which produced errors. Use ResponseType dimension for the number of different type of response. |`Transactions` |Count |Total |ResponseType, GeoType, ApiName, Authentication, TransactionType|PT1M |Yes|