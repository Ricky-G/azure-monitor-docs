---
title: Example log table queries for AADDomainServicesDirectoryServiceAccess
description:  Example queries for AADDomainServicesDirectoryServiceAccess log table
ms.topic: generated-reference
ms.service: azure-monitor
ms.author: edbaynash
author: EdB-MSFT
ms.date: 04/14/2025

# This file is automatically generated. Changes will be overwritten. Do not change this file directly. 

---

# Queries for the AADDomainServicesDirectoryServiceAccess table

For information on using these queries in the Azure portal, see [Log Analytics tutorial](/azure/azure-monitor/logs/log-analytics-tutorial). For the REST API, see [Query](/rest/api/loganalytics/query).


### Show logs from AADDomainServicesDirectoryServiceAccess table  


Lists the latest logs in AADDomainServicesDirectoryServiceAccess table, sorted by time (latest first).  

```query
AADDomainServicesDirectoryServiceAccess
| top 10 by TimeGenerated
```

