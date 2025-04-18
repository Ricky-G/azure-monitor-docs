---
title: Example log table queries for AWSVPCFlow
description:  Example queries for AWSVPCFlow log table
ms.topic: generated-reference
ms.service: azure-monitor
ms.author: edbaynash
author: EdB-MSFT
ms.date: 04/14/2025

# This file is automatically generated. Changes will be overwritten. Do not change this file directly. 

---

# Queries for the AWSVPCFlow table

For information on using these queries in the Azure portal, see [Log Analytics tutorial](/azure/azure-monitor/logs/log-analytics-tutorial). For the REST API, see [Query](/rest/api/loganalytics/query).


### Rejected IPv4 actions  


Returns 10 rejected actions of type IPv4.  

```query
AWSVPCFlow
| where Action == "REJECT"
| where Type == "IPv4"
| take 10
```

