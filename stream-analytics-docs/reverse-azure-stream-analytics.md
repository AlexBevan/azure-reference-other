---
title: "REVERSE (Azure Stream Analytics)"
description: "Returns the reverse order of a string value."
applies_to:
  - "Azure"


ms.service: stream-analytics
ms.topic: reference
ms.date: 10/22/2021
---

# REVERSE (Azure Stream Analytics)

Returns the reverse order of a string value.

## Syntax

```SQL
REVERSE ( expression )
```

## Arguments

**expression**

Is a character expression or a column of type nvarchar(max).

## Return Types

nvarchar(max)

## Examples

```SQL
SELECT
    'abcdefg' AS x,
    REVERSE('abcdefg') AS reversedX
FROM Input
```

|x|reversedX|
|-|-|
|'abcdefg'|'gfedcba'|

