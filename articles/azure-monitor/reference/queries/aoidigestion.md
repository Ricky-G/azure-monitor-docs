---
title: Example log table queries for AOIDigestion
description:  Example queries for AOIDigestion log table
ms.topic: generated-reference
ms.service: azure-monitor
ms.author: edbaynash
author: EdB-MSFT
ms.date: 04/14/2025

# This file is automatically generated. Changes will be overwritten. Do not change this file directly. 

---

# Queries for the AOIDigestion table

For information on using these queries in the Azure portal, see [Log Analytics tutorial](/azure/azure-monitor/logs/log-analytics-tutorial). For the REST API, see [Query](/rest/api/loganalytics/query).


### Row digestion errors  


All logs about rows which have failed to be digested.  

```query
AOIDigestion
| where Message startswith_cs "Failed to decode row"
| take 100
```



### Failed file digestion by source  


Breakdown of files that could not be digested by the top-level directory that they were uploaded to (typically the SiteId).  

```query
AOIDigestion
| where Message startswith_cs "Failed to digest file"
| parse FilePath with Source:string "/" *
| summarize count() by Source
```

