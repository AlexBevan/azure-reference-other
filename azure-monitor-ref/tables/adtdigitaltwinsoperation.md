---
title: Azure Monitor Logs reference - ADTDigitalTwinsOperation
description: Reference for ADTDigitalTwinsOperation table in Azure Monitor Logs.
ms.topic: reference
ms.service: azure-monitor
ms.subservice: logs
ms.author: bwren
author: bwren
ms.date: 7/2/2020
---

# ADTDigitalTwinsOperation

 Schema for Azure Digital Twins' Digital Twin operations. The Digital Twins Operation category tracks all customer requests to manage a digital twin, including CRUD on Twins and Relationships.

## Solutions

- LogManagement




## Columns

|Column|Type|Description|
|---|---|---|
|Caller IP Address|string|IP address of the requester|
|Category|string|Category of the log event|
|Correlation ID|string|Correlation ID of the operation|
|DurationMs|string|Duration of the operation in milliseconds|
|Level|string|Level of severity of the event|
|Location|string|Azure region in which the Iot Hub is located|
|OperationName|string|Operation name of the event|
|OperationVersion|string|Operation version of the event|
|RequestUri|string|The URI of the request.|
|_ResourceId|string|A unique identifier for the resource that the record is associated with|
|ResultDescription|string|Result description of the event, typically elaborates on the error|
|ResultSignature|string|Result signature of the event, typically the status code of the result|
|ResultType|string|Result type of the event, typically empty unless it's an error|
|SourceSystem|string||
|TenantId|string||
|TimeGenerated|datetime|Time at which this event is generated|
|Type|string|The name of the table|
