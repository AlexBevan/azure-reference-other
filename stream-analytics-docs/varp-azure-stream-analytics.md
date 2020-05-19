---
title: "VARP (Azure Stream Analytics) | Microsoft Docs"
description: "Returns the statistical variance for the population for all values in a group. Null values are ignored.  "
applies_to: 
  - "Azure"
services: stream-analytics
author: mamccrea


ms.service: stream-analytics
ms.topic: reference
ms.assetid: 23d50b5d-4bfc-485f-afda-adae9019ab22
caps.latest.revision: 5
ms.workload: data-services
ms.date: 04/22/2016
ms.author: mamccrea
---
# VARP (Azure Stream Analytics)
  Returns the statistical variance for the population for all values in a group. Null values are ignored.  
  
 ## Syntax  
  
```SQL   
VARP (expression )  
```  
  
## Arguments  
 **expression**  
  
 Is an expression of the exact numeric or approximate numeric data type category. VARP can be used with bigint and float columns. Aggregate functions and sub queries are not permitted.  
  
## Return Types  
 float  
  
## Examples  
  
```SQL  
SELECT System.Timestamp() AS OutTime, TollId, VARP (Toll)   
FROM Input  
GROUP BY TollId, TumblingWindow(minute,3)  
  
```  
  
  
