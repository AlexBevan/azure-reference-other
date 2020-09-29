---
title: "TopOne (Azure Stream Analytics) | Microsoft Docs"
description: "Returns the top-rank record, where rank defines the ranking position of the event in the window according to the specified ordering."
applies_to: 
  - "Azure"
services: stream-analytics
author: mamccrea


ms.service: stream-analytics
ms.topic: reference
ms.assetid: 9728630c-1c59-4349-a562-fdd98433da9d
caps.latest.revision: 6
ms.workload: data-services
ms.date: 9/20/2020
ms.author: mamccrea
---
# TopOne (Azure Stream Analytics)
  Returns the top-rank record, where rank defines the ranking position of the event in the window according to the specified ordering. Ordering/ranking is based on event columns and can be specified in ORDER BY clause.  
  
 ## Syntax  
  
```SQL
-- Aggregate Function Syntax
TopOne() OVER (ORDER BY (<column name> [ASC |DESC])+)  

-- Analytic Function Syntax
TopOne() OVER ([<PARTITION BY clause>] ORDER BY (<column name> [ASC |DESC])+ <LIMIT DURATION clause> [<WHEN clause>])  

```
  
## Arguments  
 **column_name**  
  
 Specifies the name of the column in the input event by which ordering will be done. Note that only ordering by bigint, float and datetime types are allowed.  

**OVER ([\<PARTITION BY clause> \<LIMIT DURATION clause> [\<WHEN clause>]]**

Determines the group of rows over which TopOne is applied. The PARTITION BY clause specifies that the rows with the same partition key will be grouped together. The LIMIT DURATION clause specifies how much history is included in the group. The WHEN clause specifies a boolean condition for the rows to be included in the group. See [OVER clause](over-azure-stream-analytics.md) for more details on the usage.

## Return Types
 Returns a record.

## Examples  
  
```SQL  
SELECT   
    TopOne() OVER (ORDER BY value DESC) as topEvent  
FROM input  
GROUP BY Tumbling(second, 10)  
  
```  
  
  
