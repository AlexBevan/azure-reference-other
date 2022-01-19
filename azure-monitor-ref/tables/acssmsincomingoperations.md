---
title: Azure Monitor Logs reference - ACSSMSIncomingOperations
description: Reference for ACSSMSIncomingOperations table in Azure Monitor Logs.
ms.topic: reference
ms.service: azure-monitor
ms.subservice: logs
ms.author: bwren
author: bwren
ms.date: 1/20/2022
---

# ACSSMSIncomingOperations

 Communication Services logs of incoming requests to SMS operations.

## Categories

- Azure Resources
## Solutions

- LogManagement
## Resource types

- Communication Services




## Columns

| Column | Type | Description |
| --- | --- | --- |
| CallerIpAddress | string | The caller IP address, if the operation corresponds to an API call that would come from an entity with a publicly available IP address. |
| Category | string | The log category of the event. Category is the granularity at which you can enable or disable logs on a particular resource. The properties that appear within the properties blob of an event are the same within a particular log category and resource type. |
| CorrelationId | string | The ID for correlated events. Can be used to identify correlated events between multiple tables. |
| DeliveryAttempts | int | The number of attempts made to deliver this message. |
| DurationMs | int | The duration of the operation in milliseconds. |
| IncomingMessageLength | int | The number of characters in the incoming message. |
| Level | string | The severity level of the operation. |
| Method | string | The method used in the request. |
| OperationName | string | The operation associated with log record. |
| OperationVersion | string | The API-version associated with the operation, if the operationName was performed using an API. If there is no API that corresponds to this operation, the version represents the version of that operation in case the properties associated with the operation change in the future. |
| OutgoingMessageLength | int | The number of characters in the outgoing message. |
| PhoneNumber | string | The phone number the SMS message is being sent to. |
| PlatformType | string | The platform type being used in the request. |
| _ResourceId | string | A unique identifier for the resource that the record is associated with |
| ResultDescription | string | The status text response of the result of this operation. |
| ResultSignature | string | The sub status of the operation. If this operation corresponds to a REST API call, this field is the HTTP status code of the corresponding REST call. |
| ResultType | string | The status of the operation. |
| SdkType | string | The Sdk type being used in the request. |
| SourceSystem | string |  |
| _SubscriptionId | string | A unique identifier for the subscription that the record is associated with |
| TenantId | string |  |
| TimeGenerated | datetime | The timestamp (UTC) of when the log was generated. |
| Type | string | The name of the table |
| URI | string | The URI of the request |
