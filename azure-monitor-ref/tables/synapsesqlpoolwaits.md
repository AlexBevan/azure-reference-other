---
title: Azure Monitor Logs reference - SynapseSqlPoolWaits
description: Reference for SynapseSqlPoolWaits table in Azure Monitor Logs.
ms.topic: reference
ms.service: azure-monitor
ms.subservice: logs
ms.author: robb
author: rboucher
ms.date: 4/21/2023
---

# SynapseSqlPoolWaits

 Information about the wait states encountered during execution of a SQL request/query in an Azure Synapse dedicated SQL pool, including locks and waits on transmission queues.

## Categories

- Azure Resources
## Solutions

- LogManagement
## Resource types

- Synapse Workspaces




## Columns

| Column | Type | Description |
| --- | --- | --- |
| Category | string | The category of the log. |
| LockType | string | The lock type of the SQL instance. |
| LogicalServerName | string | The logical server name of the SQL DW. |
| OperationName | string | The operation associated with log record. |
| Priority | int | The priority of the waits. |
| RequestId | string | The request ID of the waits. |
| ResourceGroup | string | The azure resourceGroup of the SQL DW. |
| _ResourceId | string | A unique identifier for the resource that the record is associated with |
| SessionId | string | The session ID of the SQL request. |
| SourceSystem | string |  |
| State | string | The State of the waits. |
| _SubscriptionId | string | A unique identifier for the subscription that the record is associated with |
| TenantId | string |  |
| TimeGenerated | datetime | The timestamp (UTC) of when the log was generated. |
| Type | string | The name of the table |
