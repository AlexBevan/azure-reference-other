---
title: Azure Monitor Logs reference - KubeServices
description: Reference for KubeServices table in Azure Monitor Logs.
ms.topic: reference
ms.service: azure-monitor
ms.subservice: logs
ms.author: robb
author: rboucher
ms.date: 5/11/2023
---

# KubeServices

 Kubernetes services and their properties

## Categories

- Containers
## Solutions

- AzureResources
- ContainerInsights
## Resource types

- Kubernetes Services
- Azure Arc Enabled Kubernetes
- Azure Arc Provisioned Clusters




## Columns

| Column | Type | Description |
| --- | --- | --- |
| ClusterId | string |  |
| ClusterIp | string |  |
| ClusterName | string |  |
| Namespace | string |  |
| _ResourceId | string | A unique identifier for the resource that the record is associated with |
| SelectorLabels | string |  |
| ServiceName | string |  |
| ServiceType | string |  |
| SourceSystem | string |  |
| _SubscriptionId | string | A unique identifier for the subscription that the record is associated with |
| TimeGenerated | datetime |  |
| Type | string | The name of the table |
