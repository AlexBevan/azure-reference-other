---
title: Azure Monitor Logs reference - CloudAppEvents
description: Reference for CloudAppEvents table in Azure Monitor Logs.
ms.topic: reference
ms.service: azure-monitor
ms.subservice: logs
ms.author: bwren
author: bwren
ms.date: 11/26/2021
---

# CloudAppEvents

 Information about activities in various cloud apps and services covered by Microsoft Cloud App Security.

## Categories

- Security
## Solutions

- Microsoft Sentinel




## Columns

| Column | Type | Description |
| --- | --- | --- |
| AccountDisplayName | string | Name displayed in the address book entry for the account user. This is usually a combination of the given name, middle initial, and surname of the user. |
| AccountObjectId | string | Unique identifier for the account in Azure AD |
| ActionType | string | Type of activity that triggered the event |
| ActivityObjects | dynamic | List of objects, such as files or folders, that were involved in the recorded activity |
| ActivityType | string | Type of activity that triggered the event |
| AdditionalFields | dynamic | Additional information about the entity or event |
| Application | string | Application that performed the recorded action |
| ApplicationId | int | Unique identifier for the application |
| City | string | City where the client IP address is geolocated |
| CountryCode | string | Two-letter code indicating the country where the client IP address is geolocated |
| DeviceType | string | Type of device based on purpose and functionality, such as network device, workstation, server, mobile, gaming console, or printer |
| IPAddress | string | IP address assigned to the device during communication |
| IsAdminOperation | bool | Indicates whether the activity was performed by an administrator |
| IsAnonymousProxy | bool | Indicates whether the IP address belongs to a known anonymous proxy |
| ISP | string | Internet service provider associated with the IP address |
| ObjectId | string | Unique identifier of the object that the recorded action was applied to |
| ObjectName | string | Name of the object that the recorded action was applied to |
| ObjectType | string | The type of object, such as a file or a folder, that the recorded action was applied to |
| OSPlatform | string | Platform of the operating system running on the device. This indicates specific operating systems, including variations within the same family, such as Windows 10 and Windows 7 |
| RawEventData | dynamic | Raw event information from the source application or service in JSON format |
| ReportId | string | Unique identifier for the event |
| SourceSystem | string |  |
| TenantId | string |  |
| TimeGenerated | datetime | Date and time (UTC) when the record was generated |
| Type | string | The name of the table |
| UserAgent | string | User agent information from the web browser or other client application |
