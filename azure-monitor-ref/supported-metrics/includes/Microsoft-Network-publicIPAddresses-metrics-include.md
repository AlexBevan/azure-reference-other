---
ms.service: azure-monitor
ms.topic: include
ms.date: 09/19/2023
ms.author: edbaynash
author: EdB-MSFT
ms.custom: Microsoft.Network/publicIPAddresses, naam
---
  
  
|Metric|Name|Unit|Aggregation|Dimensions|Time Grains|DS Export|
|---|---|---|---|---|---|---|
|Byte Count<p><p>Total number of Bytes transmitted within time period |`ByteCount` |Bytes |Total |Port, Direction|PT1M |Yes|
|Inbound bytes dropped DDoS<p><p>Inbound bytes dropped DDoS |`BytesDroppedDDoS` |BytesPerSecond |Maximum |No Dimensions|PT1M |Yes|
|Inbound bytes forwarded DDoS<p><p>Inbound bytes forwarded DDoS |`BytesForwardedDDoS` |BytesPerSecond |Maximum |No Dimensions|PT1M |Yes|
|Inbound bytes DDoS<p><p>Inbound bytes DDoS |`BytesInDDoS` |BytesPerSecond |Maximum |No Dimensions|PT1M |Yes|
|Inbound SYN packets to trigger DDoS mitigation<p><p>Inbound SYN packets to trigger DDoS mitigation |`DDoSTriggerSYNPackets` |CountPerSecond |Maximum |No Dimensions|PT1M |Yes|
|Inbound TCP packets to trigger DDoS mitigation<p><p>Inbound TCP packets to trigger DDoS mitigation |`DDoSTriggerTCPPackets` |CountPerSecond |Maximum |No Dimensions|PT1M |Yes|
|Inbound UDP packets to trigger DDoS mitigation<p><p>Inbound UDP packets to trigger DDoS mitigation |`DDoSTriggerUDPPackets` |CountPerSecond |Maximum |No Dimensions|PT1M |Yes|
|Under DDoS attack or not<p><p>Under DDoS attack or not |`IfUnderDDoSAttack` |Count |Maximum |No Dimensions|PT1M |Yes|
|Packet Count<p><p>Total number of Packets transmitted within time period |`PacketCount` |Count |Total |Port, Direction|PT1M |Yes|
|Inbound packets dropped DDoS<p><p>Inbound packets dropped DDoS |`PacketsDroppedDDoS` |CountPerSecond |Maximum |No Dimensions|PT1M |Yes|
|Inbound packets forwarded DDoS<p><p>Inbound packets forwarded DDoS |`PacketsForwardedDDoS` |CountPerSecond |Maximum |No Dimensions|PT1M |Yes|
|Inbound packets DDoS<p><p>Inbound packets DDoS |`PacketsInDDoS` |CountPerSecond |Maximum |No Dimensions|PT1M |Yes|
|SYN Count<p><p>Total number of SYN Packets transmitted within time period |`SynCount` |Count |Total |Port, Direction|PT1M |Yes|
|Inbound TCP bytes dropped DDoS<p><p>Inbound TCP bytes dropped DDoS |`TCPBytesDroppedDDoS` |BytesPerSecond |Maximum |No Dimensions|PT1M |Yes|
|Inbound TCP bytes forwarded DDoS<p><p>Inbound TCP bytes forwarded DDoS |`TCPBytesForwardedDDoS` |BytesPerSecond |Maximum |No Dimensions|PT1M |Yes|
|Inbound TCP bytes DDoS<p><p>Inbound TCP bytes DDoS |`TCPBytesInDDoS` |BytesPerSecond |Maximum |No Dimensions|PT1M |Yes|
|Inbound TCP packets dropped DDoS<p><p>Inbound TCP packets dropped DDoS |`TCPPacketsDroppedDDoS` |CountPerSecond |Maximum |No Dimensions|PT1M |Yes|
|Inbound TCP packets forwarded DDoS<p><p>Inbound TCP packets forwarded DDoS |`TCPPacketsForwardedDDoS` |CountPerSecond |Maximum |No Dimensions|PT1M |Yes|
|Inbound TCP packets DDoS<p><p>Inbound TCP packets DDoS |`TCPPacketsInDDoS` |CountPerSecond |Maximum |No Dimensions|PT1M |Yes|
|Inbound UDP bytes dropped DDoS<p><p>Inbound UDP bytes dropped DDoS |`UDPBytesDroppedDDoS` |BytesPerSecond |Maximum |No Dimensions|PT1M |Yes|
|Inbound UDP bytes forwarded DDoS<p><p>Inbound UDP bytes forwarded DDoS |`UDPBytesForwardedDDoS` |BytesPerSecond |Maximum |No Dimensions|PT1M |Yes|
|Inbound UDP bytes DDoS<p><p>Inbound UDP bytes DDoS |`UDPBytesInDDoS` |BytesPerSecond |Maximum |No Dimensions|PT1M |Yes|
|Inbound UDP packets dropped DDoS<p><p>Inbound UDP packets dropped DDoS |`UDPPacketsDroppedDDoS` |CountPerSecond |Maximum |No Dimensions|PT1M |Yes|
|Inbound UDP packets forwarded DDoS<p><p>Inbound UDP packets forwarded DDoS |`UDPPacketsForwardedDDoS` |CountPerSecond |Maximum |No Dimensions|PT1M |Yes|
|Inbound UDP packets DDoS<p><p>Inbound UDP packets DDoS |`UDPPacketsInDDoS` |CountPerSecond |Maximum |No Dimensions|PT1M |Yes|
|Data Path Availability<p><p>Average IP Address availability per time duration |`VipAvailability` |Count |Average |Port|PT1M |Yes|