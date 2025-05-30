---
title: Example log table queries for TOUserAudits
description:  Example queries for TOUserAudits log table
ms.topic: generated-reference
ms.service: azure-monitor
ms.author: edbaynash
author: EdB-MSFT
ms.date: 04/14/2025

# This file is automatically generated. Changes will be overwritten. Do not change this file directly. 

---

# Queries for the TOUserAudits table

For information on using these queries in the Azure portal, see [Log Analytics tutorial](/azure/azure-monitor/logs/log-analytics-tutorial). For the REST API, see [Query](/rest/api/loganalytics/query).


### Auditing ToolchainOrchestrator Operations  


Lists of audit Toolchain orchestrator operations.  

```query
TOUserAudits
| where Message !startswith_cs "Request" 
| order by EdgeLocation, TimeGenerated desc
| project EdgeLocation, TimeGenerated, User, Message, OperatingResourceId, OperatingResourceK8SId, OperationName
| take 100
```



### Auditing ToolchainOrchestrator API requests  


Lists of audit Toolchain orchestrator api requests.  

```query
TOUserAudits
| where Message startswith_cs "Request" 
| order by EdgeLocation, TimeGenerated desc
| project EdgeLocation, TimeGenerated, User, Message, OperatingResourceId, OperatingResourceK8SId, OperationName
| take 100
```

