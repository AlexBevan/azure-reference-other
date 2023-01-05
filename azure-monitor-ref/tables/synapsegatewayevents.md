---
title: Azure Monitor Logs reference - SynapseGatewayEvents
description: Reference for SynapseGatewayEvents table in Azure Monitor Logs.
ms.topic: reference
ms.service: azure-monitor
ms.subservice: logs
ms.author: bwren
author: bwren
ms.date: 1/5/2023
---

# SynapseGatewayEvents

 Logs for all user requests that go through gateway on synapse.

## Solutions

- LogManagement




## Columns

| Column | Type | Description |
| --- | --- | --- |
| Category | string | The category of the log. |
| CorrelationId | string | A GUID used to group together a set of related events. |
| Identity | dynamic | A JSON blob that describes the identity of the user or application that performed the operation. |
| Location | string | The region of the resource emitting the event. |
| OperationName | string | The operation associated with log record. |
| OperationVersion | string | The API Version of the operation. |
| RequestUri | string | The request URI for this query. |
| _ResourceId | string | A unique identifier for the resource that the record is associated with |
| ResultDescription | string | The static text description of this operation. |
| ResultSignature | string | The sub status of the event |
| ResultType | string | Status of the event. |
| SourceSystem | string |  |
| _SubscriptionId | string | A unique identifier for the subscription that the record is associated with |
| TenantId | string |  |
| TimeGenerated | datetime | The timestamp (UTC) of when the log was generated. |
| Type | string | The name of the table |
