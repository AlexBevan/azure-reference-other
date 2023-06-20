---
title: Azure Monitor Logs reference - DeviceTvmSecureConfigurationAssessment
description: Reference for DeviceTvmSecureConfigurationAssessment table in Azure Monitor Logs.
ms.topic: reference
ms.service: azure-monitor
ms.subservice: logs
ms.author: robb
author: rboucher
ms.date: 6/20/2023
---

# DeviceTvmSecureConfigurationAssessment

 Threat & vulnerability management assessment events, indicating the status of various security configurations on devices.

## Categories

- Security
## Solutions

- Microsoft Sentinel




## Columns

| Column | Type | Description |
| --- | --- | --- |
| _BilledSize | real |  |
| ConfigurationCategory | string | Category or grouping to which the configuration belongs |
| ConfigurationId | string | Unique identifier for a specific configuration |
| ConfigurationImpact | real | Rated impact of the configuration to the overall configuration score (1-10) |
| ConfigurationSubcategory | string | Subcategory or subgrouping to which the configuration belongs. In many cases, this describes specific capabilities or features. |
| Context | dynamic | Machine data configuration context |
| DeviceId | string | Unique identifier for the device in the service |
| DeviceName | string | Fully qualified domain name (FQDN) of the device |
| IsApplicable | bool | Indicates whether the configuration or policy is applicable |
| _IsBillable | string |  |
| IsCompliant | bool | Indicates whether the configuration or policy is properly configured |
| IsExpectedUserImpact | bool | Indicates if user impact is expected when configuration applied |
| OSPlatform | string | Platform of the operating system running on the device. This indicates specific operating systems, including variations within the same family, such as Windows 10 and Windows 7 |
| SourceSystem | string | The type of agent the event was collected by. For example, *OpsManager* for Windows agent, either direct connect or Operations Manager, *Linux* for all Linux agents, or *Azure* for Azure Diagnostics |
| TenantId | string | The Log Analytics workspace ID |
| TimeGenerated | datetime | Date and time when the record was generated |
| Timestamp | datetime | Date and time when the record was generated |
| Type | string | The name of the table |
