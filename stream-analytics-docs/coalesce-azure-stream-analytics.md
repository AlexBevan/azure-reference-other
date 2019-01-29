---
title: "COALESCE (Azure Stream Analytics) | Microsoft Docs"
description: "Evaluates the arguments in order and returns the value of the first expression that initially does not evaluate to NULL."
services: stream-analytics
author: mamccrea
ms.service: stream-analytics
ms.topic: reference
ms.date: 01/28/2019
ms.author: mamccrea
---
# COALESCE (Azure Stream Analytics)
  Evaluates the arguments in order and returns the value of the first expression that initially does not evaluate to NULL. 

## Syntax  
  
```SQL   
COALESCE ( expression1, expression2,  [ ,…n ] )
```  
  
## Arguments

**expression**  
  
An expression of any type.
  
## Return Types  

The type of the first non-null expression.
  
## Examples  
  
```SQL  
SELECT COALESCE(a, b) AS result FROM input
```  
  
|Expression|Result|
|----------|------|
|COALESCE(0, ‘a’)|0|
|COALESCE(NULL, ‘a’)|‘a’|
|COALESCE(NULL, NULL)|null|
|COALESCE(NULL, NULL, 2, NULL)|2|