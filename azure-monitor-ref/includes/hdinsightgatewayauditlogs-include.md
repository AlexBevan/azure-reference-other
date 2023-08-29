---
ms.service: azure-monitor
ms.topic: include
ms.date: 08/28/2023
ms.author: edbaynash
author: EdB-MSFT
ms.custom: HDInsightGatewayAuditLogs
---


| Column | Type | Description |
|---|---|---|
| AccessRequestCount | real | Number of login requests associated with the user. |
| _BilledSize | real | The record size in bytes |
| ClusterDnsName | string | The DNS name of the cluster. |
| ErrorMessage | string | Any error message associated with the login attempt. |
| _IsBillable | string | Specifies whether ingesting the data is billable. When _IsBillable is `false` ingestion isn't billed to your Azure account |
| _ResourceId | string | A unique identifier for the resource that the record is associated with |
| SourceSystem | string | The type of agent the event was collected by. For example, `OpsManager` for Windows agent, either direct connect or Operations Manager, `Linux` for all Linux agents, or `Azure` for Azure Diagnostics |
| Status | string | The outcome of the login attempt. |
| _SubscriptionId | string | A unique identifier for the subscription that the record is associated with |
| TenantId | string | The Log Analytics workspace ID |
| TimeGenerated | datetime | The timestamp (UTC) of when the log was generated. |
| Type | string | The name of the table |
| UserName | string | The username used for the login attempt. |
