---
title: Azure Monitor Logs reference - ASRJobs
description: Reference for ASRJobs table in Azure Monitor Logs.
ms.topic: reference
ms.service: azure-monitor
ms.subservice: logs
ms.author: edbaynash
author: EdB-MSFT
ms.date: 08/28/2023
---

# ASRJobs

This table contains records of Azure Site Recovery (ASR) jobs such as failover, test failover, reprotection etc., with key details for monitoring and diagnostics, such as the replicated item information, duration, status, description and so on. Whenever an ASR job is completed (i.e., succeeded or failed), a corresponding record for the job is sent to this table. You can view history of ASR jobs by querying this table over a larger time range, provided your workspace has the required retention configured.

## Categories

- Audit
## Solutions

- LogManagement
## Resource types

- Recovery Services Vaults

            


## Columns
  
[!INCLUDE [asrjobs](../includes/asrjobs-include.md)]
