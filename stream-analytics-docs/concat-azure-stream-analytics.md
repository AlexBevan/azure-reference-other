---
title: "CONCAT (Azure Stream Analytics)"
description: "Returns a string that is the result of concatenating two or more string values. "
applies_to: 
  - "Azure"


ms.service: stream-analytics
ms.topic: reference
ms.date: 04/22/2016
---
# CONCAT (Azure Stream Analytics)
  Returns a string that is the result of concatenating two or more string values.  
  
 ## Syntax  
  
```SQL  
CONCAT ( string_value1, string_value2 [, string_valueN ] )  
```  
  
## Arguments  
 **string_value**  
  
 A string value to concatenate to the other values.  
  
## Return Types  
 nvarchar(max)

## Remarks
CONCAT implicitly converts null values to empty strings. If CONCAT receives arguments with all NULL values, it will return an empty string.

## Examples  
  
```SQL 
SELECT TollId, EntryTime, CONCAT ( 'Make:', Make, ' And Model:', Model) AS MakeModel, LicensePlate  
FROM Input TIMESTAMP BY EntryTime  
WHERE Toll > 5  
  
```  
  
  
