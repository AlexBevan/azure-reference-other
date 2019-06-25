---
title: "CASE (Azure Stream Analytics) | Microsoft Docs"
description: "Evaluates a list of conditions and returns one of multiple possible result expressions."
applies_to: 
  - "Azure"
services: stream-analytics
author: mamccrea
manager: kfile

ms.service: stream-analytics
ms.topic: reference
ms.assetid: 7c32501d-0e3e-49e8-8c84-61d33830e355
caps.latest.revision: 7
ms.workload: data-services
ms.date: 04/22/2016
ms.author: mamccrea
---

# CASE (Azure Stream Analytics)

  Evaluates a list of conditions and returns one of multiple possible result expressions.  
  
 The CASE expression has two formats:  
  
- The simple CASE expression compares an expression to a set of simple expressions to determine the result.  
  
- The searched CASE expression evaluates a set of Boolean expressions to determine the result.  
  
 Both formats require an ELSE argument.  
  
 CASE can be used in any statement or clause that allows a valid expression. For example, you can use CASE in expressions such as SELECT and in clauses such as WHERE and HAVING.  
  
## Syntax  
  
 Simple CASE expression:  
  
```SQL
CASE input_expression
     WHEN when_expression THEN result_expression [ ...n ] 
     ELSE else_result_expression
END  
```

 Searched CASE expression:  
  
```SQL  
CASE  
     WHEN Boolean_expression THEN result_expression [ ...n ]
     ELSE else_result_expression  
END  
```  

## Arguments

### input_expression

Is the expression evaluated when the simple CASE format is used. The evaluated value is compared against the *when_expression*.

### WHEN when_expression

Is the expression to which *input_expression* is compared when using the simple CASE format. The types of the *when_expressions* do not necessarily have to match.

### WHEN boolean_expression

Is the boolean expression evaluated when using the searched CASE format. If this expression evaluates to true, then the corresponding *result_expression* is returned.

### THEN result_expression

Is the expression returned when *input_expression* equals *when_expression* (in the simple CASE format) or when *boolean_expression* evaluates to true (in the searched CASE format).

### ELSE else_result_expression

Is the expression returned if none of the conditions evaluated to TRUE.

## Return type

Is the highest precedence type from the set of types in *result_expression*(s) and *else_result_expression*.

## Examples

Using select with a simple CASE expression:

```SQL
  SELECT
    CASE vehicleType
      WHEN 'S' THEN 'Sedan'
      WHEN 'T' THEN 'Truck'
      WHEN 'V' THEN 'Van'
      ELSE NULL
    END as vehicleTypeName
  FROM vehicles
```

Using select with searched CASE expression:

```SQL
  SELECT
    CASE
      WHEN temperature < 60 THEN 'Alert'
      ELSE 'OK'
    END as currentStatus
  FROM sensor
```
