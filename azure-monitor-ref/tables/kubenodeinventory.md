---
title: Azure Monitor Logs reference - KubeNodeInventory
description: Reference for KubeNodeInventory table in Azure Monitor Logs.
ms.topic: reference
ms.service: azure-monitor
ms.subservice: logs
ms.author: robb
author: rboucher
ms.date: 3/31/2023
---

# KubeNodeInventory

 Details for nodes that are part of kubernetes cluster.

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
| ClusterName | string |  |
| Computer | string |  |
| CreationTimeStamp | datetime |  |
| DockerVersion | string |  |
| KubeletVersion | string |  |
| KubeProxyVersion | string |  |
| KubernetesProviderID | string |  |
| Labels | string |  |
| LastTransitionTimeReady | datetime |  |
| OperatingSystem | string |  |
| _ResourceId | string | A unique identifier for the resource that the record is associated with |
| SourceSystem | string |  |
| Status | string |  |
| _SubscriptionId | string | A unique identifier for the subscription that the record is associated with |
| TimeGenerated | datetime |  |
| Type | string | The name of the table |
