---
title: Azure Monitor Logs reference - WebPubSubMessaging
description: Reference for WebPubSubMessaging table in Azure Monitor Logs.
ms.topic: reference
ms.service: azure-monitor
ms.subservice: logs
ms.author: bwren
author: bwren
ms.date: 3/25/2022
---

# WebPubSubMessaging

 Messaging logs provide tracing information for the Azure Web PubSub hub messages received and sent via Azure Web PubSub service. For example, tracing ID and message type of the message. Typically the message is recorded when it arrives at or leaves from service and is helpful for troubleshooting message-related issues.

## Categories

- Azure Resources
## Solutions

- LogManagement
## Resource types

- SignalR Service WebPubSub




## Columns

| Column | Type | Description |
| --- | --- | --- |
| CallerIpAddress | string | The IP of the client or server connects to Web PubSub service. |
| ConnectionId | string | The unique identifier of the connection connected to service. |
| Level | string | The level of the log. Can be 'Informational', 'Warning', 'Error' or 'Critical'. |
| Location | string | The location of Azure Web PubSub service. |
| Message | string | The message of the log event. It provides details about the event. |
| OperationName | string | The operation of the log event. It can be used to filter the log based on a specific operation name. |
| _ResourceId | string | A unique identifier for the resource that the record is associated with |
| SourceSystem | string |  |
| _SubscriptionId | string | A unique identifier for the subscription that the record is associated with |
| TenantId | string |  |
| TimeGenerated | datetime | The timestamp (UTC) of the log. |
| TraceId | string | The unique identifier of the invocations. It's used for tracing invocations. |
| Type | string | The name of the table |
| UserId | string | The unique identifier of the user. It is defined by the client or app server. |
