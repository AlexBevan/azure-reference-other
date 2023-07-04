---
title: Azure Monitor Logs reference - MicrosoftGraphActivityLogs
description: Reference for MicrosoftGraphActivityLogs table in Azure Monitor Logs.
ms.topic: reference
ms.service: azure-monitor
ms.subservice: logs
ms.author: robb
author: rboucher
ms.date: 7/3/2023
---

# MicrosoftGraphActivityLogs

 Microsoft Graph Activity Logs provide details of API requests made to Microsoft Graph for resources in the tenant.

## Categories

- Audit
- Security
## Solutions

- LogManagement




## Columns

| Column | Type | Description |
| --- | --- | --- |
| AadTenantId | string | The Azure AD tenant ID. |
| ApiVersion | string | The API version of the event. |
| AppId | string | The identifier for the application. |
| _BilledSize | real |  |
| ClientRequestId | string | Optional. The client request identifier when sent. If no client request identifier is sent, the value will be equal to the operation identifier. |
| DurationMs | int | The duration of the request in milliseconds. |
| IpAddress | string | The IP address of the client from where the request occurred. |
| _IsBillable | string |  |
| Location | string | The name of the region that served the request. |
| OperationId | string | The identifier for the batch. For non-batched requests, this will be unique per request. For batched requests, this will be the same for all requests in the batch. |
| RequestId | string | The identifier representing the request. |
| RequestMethod | string | The HTTP method of the event. |
| RequestUri | string | The URI of the request. |
| ResponseSizeBytes | int | The size of the response in Bytes. |
| ResponseStatusCode | int | The HTTP response status code for the event. |
| Roles | string | The roles in token claims. |
| Scopes | string | The scopes in token claims. |
| ServicePrincipalId | string | The identifier of the servicePrincipal making the request. |
| SignInActivityId | string | The identifier representing the sign-in activitys. |
| SourceSystem | string | The type of agent the event was collected by. For example, *OpsManager* for Windows agent, either direct connect or Operations Manager, *Linux* for all Linux agents, or *Azure* for Azure Diagnostics |
| TenantId | string | The Log Analytics workspace ID |
| TimeGenerated | datetime | The date and time the request was received. |
| TokenIssuedAt | datetime | The timestamp the token was issued at. |
| Type | string | The name of the table |
| UserAgent | string | The user agent information related to request. |
| UserId | string | The identifier of the user making the request. |
