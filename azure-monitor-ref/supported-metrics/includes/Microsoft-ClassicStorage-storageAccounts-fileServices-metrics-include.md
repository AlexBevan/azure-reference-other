---
ms.service: azure-monitor
ms.topic: include
ms.date: 09/19/2023
ms.author: edbaynash
author: EdB-MSFT
ms.custom: Microsoft.ClassicStorage/storageAccounts/fileServices, arm
---
  
  
|Metric|Name|Unit|Aggregation|Dimensions|Time Grains|DS Export|
|---|---|---|---|---|---|---|
|Availability<p><p>The percentage of availability for the storage service or the specified API operation. Availability is calculated by taking the TotalBillableRequests value and dividing it by the number of applicable requests, including those that produced unexpected errors. All unexpected errors result in reduced availability for the storage service or the specified API operation. |`Availability` |Percent |Average, Minimum, Maximum |GeoType, ApiName, Authentication, FileShare|PT1M |Yes|
|Egress<p><p>The amount of egress data, in bytes. This number includes egress from an external client into Azure Storage as well as egress within Azure. As a result, this number does not reflect billable egress. |`Egress` |Bytes |Total, Average, Minimum, Maximum |GeoType, ApiName, Authentication, FileShare|PT1M |Yes|
|File Capacity<p><p>The amount of storage used by the storage account's File service in bytes. |`FileCapacity` |Bytes |Average |FileShare|PT1H |No|
|File Count<p><p>The number of file in the storage account's File service. |`FileCount` |Count |Average |FileShare|PT1H |No|
|File Share Count<p><p>The number of file shares in the storage account's File service. |`FileShareCount` |Count |Average |No Dimensions|PT1H |No|
|File share quota size<p><p>The upper limit on the amount of storage that can be used by Azure Files Service in bytes. |`FileShareQuota` |Bytes |Average |FileShare|PT1H |No|
|File Share Snapshot Count<p><p>The number of snapshots present on the share in storage account's Files Service. |`FileShareSnapshotCount` |Count |Average |FileShare|PT1H |No|
|File Share Snapshot Size<p><p>The amount of storage used by the snapshots in storage account's File service in bytes. |`FileShareSnapshotSize` |Bytes |Average |FileShare|PT1H |No|
|Ingress<p><p>The amount of ingress data, in bytes. This number includes ingress from an external client into Azure Storage as well as ingress within Azure. |`Ingress` |Bytes |Total, Average, Minimum, Maximum |GeoType, ApiName, Authentication, FileShare|PT1M |Yes|
|Success E2E Latency<p><p>The end-to-end latency of successful requests made to a storage service or the specified API operation, in milliseconds. This value includes the required processing time within Azure Storage to read the request, send the response, and receive acknowledgment of the response. |`SuccessE2ELatency` |Milliseconds |Average, Minimum, Maximum |GeoType, ApiName, Authentication, FileShare|PT1M |Yes|
|Success Server Latency<p><p>The latency used by Azure Storage to process a successful request, in milliseconds. This value does not include the network latency specified in SuccessE2ELatency. |`SuccessServerLatency` |Milliseconds |Average, Minimum, Maximum |GeoType, ApiName, Authentication, FileShare|PT1M |Yes|
|Transactions<p><p>The number of requests made to a storage service or the specified API operation. This number includes successful and failed requests, as well as requests which produced errors. Use ResponseType dimension for the number of different type of response. |`Transactions` |Count |Total |ResponseType, GeoType, ApiName, Authentication, FileShare|PT1M |Yes|