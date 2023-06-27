---
title: Azure Monitor Logs reference - UserPeerAnalytics
description: Reference for UserPeerAnalytics table in Azure Monitor Logs.
ms.topic: reference
ms.service: azure-monitor
ms.subservice: logs
ms.author: robb
author: rboucher
ms.date: 6/27/2023
---

# UserPeerAnalytics

 This analytics table, for a given user, provides a ranked list of peers. For example, if the user is Jane Smith, Peer Analytics calculates all of Jane's peers based on her mailing list, security groups, etc and provides the top 20 of her peers.

## Categories

- Security
## Solutions

- Microsoft Sentinel UEBA




## Columns

| Column | Type | Description |
| --- | --- | --- |
| AADTenantId | string | Unique identifier of the Azure Tenant |
| _BilledSize | real |  |
| _IsBillable | string |  |
| PeerUserId | string | Unique identifier of the peer of the primary user |
| PeerUserName | string | User name of the peer of the primary user |
| PeerUserPrincipalName | string | User principal name of the peer of the primary user |
| Rank | int | Rank of the peer with respect to the primary user |
| _ResourceId | string | A unique identifier for the resource that the record is associated with |
| SourceSystem | string | The type of agent the event was collected by. For example, *OpsManager* for Windows agent, either direct connect or Operations Manager, *Linux* for all Linux agents, or *Azure* for Azure Diagnostics |
| _SubscriptionId | string | A unique identifier for the subscription that the record is associated with |
| TenantId | string | The Log Analytics workspace ID |
| TimeGenerated | datetime | Timestamp when the peer analytics is calculated |
| Type | string | The name of the table |
| UserId | string | Unique identifier of the primary user |
| UserName | string | User name of the primary user |
| UserPrincipalName | string | User principal name of the primary user |
