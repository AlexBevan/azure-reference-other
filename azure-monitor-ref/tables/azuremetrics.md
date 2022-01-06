---
title: Azure Monitor Logs reference - AzureMetrics
description: Reference for AzureMetrics table in Azure Monitor Logs.
ms.topic: reference
ms.service: azure-monitor
ms.subservice: logs
ms.author: bwren
author: bwren
ms.date: 1/6/2022
---

# AzureMetrics

 Metric data emitted by Azure services that measure their health and performance.

## Categories

- Azure Resources
## Solutions

- LogManagement
## Resource types

- App Services
- Azure Database for MySQL Servers
- SQL Databases
- SQL Servers
- SQL Managed Instances
- Data Share
- Power BI Embedded
- Azure Database for PostgreSQL Servers
- Data Lake Analytics
- Data factories
- Automation account
- API Management services
- Logic Apps
- Service Fabric Clusters
- IoT Hub
- Data Lake Storage Gen1
- Azure Database for PostgreSQL Servers V2
- Azure Database for PostgreSQL Flexible Servers
- Azure Database for MariaDB Servers
- Bastions
- Stream Analytics jobs
- Search Services
- Virtual Networks
- Virtual Private Network Gateways
- Virtual Network Gateways
- Traffic Manager Profiles
- Public IP Addresses
- Network Security Groups
- Network Interfaces
- Front Doors
- ExpressRoute Circuits
- Application Gateways
- Event Hubs
- Device Provisioning Services
- Azure Monitor autoscale settings
- Azure Databricks Services
- Azure Arc enabled Kubernetes
- Virtual Machine Scale Sets
- Desktop Virtualization workspaces
- Desktop Virtualization Application Groups
- Desktop Virtualization Host Pools
- Synapse Workspaces
- Virtual machines
- Machine Learning
- Microsoft Connected Vehicle Platform
- Microsoft Connected Cache
- Azure Traffic Collector
- Kubernetes Services
- Firewalls
- Project CI Workspace
- Azure Cosmos DB
- Communication Services
- Azure Cache for Redis
- Time Series Insights Environments
- Azure API for FHIR
- Workload Monitor
- Batch Accounts
- System Center Virtual Machine Manager
- Azure Stack HCI
- VMware
- Event Grid Topics
- Event Grid Domains
- Azure Blockchain Service
- Azure AD Domain Services
- Azure Data Explorer Clusters
- Container Registries
- SignalR
- Storage Accounts
- Key Vaults
- Cognitive Services
- Media Services
- Azure Spring Cloud
- Analysis Services
- Service Bus




## Columns

| Column | Type | Description |
| --- | --- | --- |
| Average | real |  |
| CallerIpAddress | string | Deprecated |
| Category | string | Deprecated |
| Confidence | string | Deprecated |
| CorrelationId | string | Deprecated |
| Count | real | Number of samples collected during the time range. Can be used to determine the number of values that contributed to the average value. |
| Description | string | Deprecated |
| DurationMs | long | Deprecated |
| FirstReportedDateTime | string | Deprecated |
| IndicatorThreatType | string | Deprecated |
| IsActive | string | Deprecated |
| LastReportedDateTime | string | Deprecated |
| MaliciousIP | string | Deprecated |
| Maximum | real | Maximum value collected during in the time range. |
| MetricName | string | Display name of the metric. |
| Minimum | real | Minimum value collected during in the time range. |
| OperationName | string | Deprecated |
| OperationVersion | string | Deprecated |
| RemoteIPCountry | string | Deprecated |
| RemoteIPLatitude | real | Deprecated |
| RemoteIPLongitude | real | Deprecated |
| Resource | string | Resource name of the Azure resource reporting the metric. |
| ResourceGroup | string | Resource group name of the Azure resource reporting the metric. |
| _ResourceId | string | A unique identifier for the resource that the record is associated with |
| ResourceId | string | Resource ID of the Azure resource reporting the metric. Same as _ResourceId present for backward compatibility reasons. _ResourceId should be used |
| ResourceProvider | string | Resource provider of the Azure resource reporting the metric. |
| ResultDescription | string | Deprecated |
| ResultSignature | string | Deprecated |
| ResultType | string | Reduces the set of data collected. The syntax allowed depends on the operation. See the operation's description for details. |
| Severity | int | Deprecated |
| SourceSystem | string | OpsManagerfor all records in this table. |
| SubscriptionId | string | Subscription id of the Azure resource reporting the metric. |
| _SubscriptionId | string | A unique identifier for the subscription that the record is associated with |
| TimeGenerated | datetime | Date and time the record was created. |
| TimeGrain | string | Time grain of the metric e.g. PT1M |
| TLPLevel | string | Deprecated |
| Total | real | Sum of all of the values in the time range. |
| Type | string | The name of the table |
| UnitName | string | Unit of the metric. Examples include Seconds Percent Bytes. |
