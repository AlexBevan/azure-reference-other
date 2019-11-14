---
title: "Tumbling Window (Azure Stream Analytics) | Microsoft Docs"
description: "Tumbling windows are a series of fixed-sized, non-overlapping and contiguous time intervals."
applies_to: 
  - "Azure"
services: stream-analytics
author: mamccrea
ms.author: mamccrea
ms.service: stream-analytics
ms.topic: reference
ms.assetid: cfc2fb3b-0e8e-4b5e-b3ba-8ca6fea61c17
ms.workload: data-services
ms.date: 06/21/2019
---
# Tumbling Window (Azure Stream Analytics)
  Tumbling windows are a series of fixed-sized, non-overlapping and contiguous time intervals. The following diagram illustrates a stream with a series of events and how they are mapped into 10-second tumbling windows.  
  
 ![Stream Analytics tumbling window 5 mins](media/tumbling-window-azure-stream-analytics/streamanalytics-tumblingwindow5mins.png "Stream Analytics tumbling window 5 mins")  
  
 ## Syntax  
  
```SQL   
{TUMBLINGWINDOW | TUMBLING} ( timeunit  , windowsize, [offsetsize] )  
{TUMBLINGWINDOW | TUMBLING} ( Duration( timeunit  , windowsize ), [Offset(timeunit  , offsetsize)] )  
  
```  

> [!NOTE]  
>  The Tumbling Window can be used in the above two ways. To allow consistency with the Hopping Window, the Duration function can also be used with all types of windows to specify the window size. The window duration must be a positive float constant.  
  
## Arguments  
 **timeunit**  
  
 Is the unit of time for the windowsize. The following table lists all valid timeunit arguments.  
  
|Timeunit|Abbreviations|  
|--------------|-------------------|  
|day|dd, d|  
|hour|hh|  
|minute|mi, n|  
|second|ss, s|  
|millisecond|ms|  
|microsecond|mcs|  
  
 **windowsize**  
  
 A big integer which describes the size of the window. The windowsize is static and cannot be changed dynamically at runtime.  
  
 The maximum size of the window is 7 days.  
  
 **offsetsize**  
  
 By default, tumbling windows are inclusive in the end of the window and exclusive in the beginning – for example 12:00 PM – 1:00 PM window will include events that happened exactly at 1:00 PM, but will not include events that happened at 12:00PM (these events will be part of 11:00 AM – 12:00 PM window).  
  
 The Offset parameter can be used to change this behavior and include the events in the beginning of the window and exclude the ones that happened in the end.  
  
## Examples  
  
```SQL  
SELECT System.Timestamp() AS WindowEnd, TollId, COUNT(*)  
FROM Input TIMESTAMP BY EntryTime  
GROUP BY TollId, TumblingWindow(Duration(hour, 1), Offset(millisecond, -1))
```

```SQL
SELECT 'reset' AS command
INTO
    alert
FROM
    temperature TIMESTAMP BY timeCreated
GROUP BY TumblingWindow(second,15)
HAVING Avg(machine.temperature) > 25
```
  
## See Also  
 [Hopping Window](hopping-window-azure-stream-analytics.md)   
 [Sliding Window](sliding-window-azure-stream-analytics.md)   
 [Windowing](windowing-azure-stream-analytics.md)  
  
  
