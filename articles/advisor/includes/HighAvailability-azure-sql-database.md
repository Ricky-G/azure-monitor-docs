---
ms.service: azure
ms.topic: include
ms.date: 06/10/2025
author: kanika1894
ms.author: kapasrij
ms.custom: HighAvailability Azure SQL Database
  
# NOTE:  This content is automatically generated using API calls to Azure. Any edits made on these files will be overwritten in the next run of the script. 
  
---
  
## Azure SQL Database  
  
<!--2ea11bcb-dfd0-48dc-96f0-beba578b989a_begin-->

#### Enable cross region disaster recovery for SQL Database  
  
Enable cross region disaster recovery for Azure SQL Database for business continuity in the event of regional outage.  
  
**Potential benefits**: Enabling disaster recovery creates a continuously synchronized readable secondary database for a primary database.  

**Impact:** High
  
For more information, see [Cloud Business Continuity - Disaster Recovery - Azure SQL Database](https://aka.ms/sqldb_dr_overview)  

ResourceType: microsoft.sql/servers/databases  
Recommendation ID: 2ea11bcb-dfd0-48dc-96f0-beba578b989a  
Subcategory: DisasterRecovery

<!--2ea11bcb-dfd0-48dc-96f0-beba578b989a_end-->






<!--807e58d0-e385-41ad-987b-4a4b3e3fb563_begin-->

#### Enable zone redundancy for Azure SQL Database to achieve high availability and resiliency.  
  
To achieve high availability and resiliency, enable zone redundancy for the SQL database or elastic pool to use availability zones and ensure the database or elastic pool is resilient to zonal failures.  
  
**Potential benefits**: Enabling zone redundancy ensures Azure SQL Database is resilient to zonal hardware and software failures and the recovery is transparent to applications.  

**Impact:** High
  
For more information, see [Availability through local and zone redundancy - Azure SQL Database ](/azure/azure-sql/database/high-availability-sla?view=azuresql&tabs=azure-powershell#zone-redundant-availability)  

ResourceType: microsoft.sql/servers/databases  
Recommendation ID: 807e58d0-e385-41ad-987b-4a4b3e3fb563  
Subcategory: HighAvailability

<!--807e58d0-e385-41ad-987b-4a4b3e3fb563_end-->

<!--e1967ca0-c0c3-4ae2-b69b-13d5676a4b18_begin-->

#### Enable cross region disaster recovery for SQL Managed Instance  
  
Consider deploying a failover group for the SQL Managed Instance to allow business continuity in different Azure regions to deal with a regional outage.  
  
**Potential benefits**: Ensure business continuity through regional redundancy.  

**Impact:** High
  
For more information, see [Failover groups overview & best practices - Azure SQL Managed Instance](https://aka.ms/instanceFailoverGroups)  

ResourceType: microsoft.sql/managedinstances  
Recommendation ID: e1967ca0-c0c3-4ae2-b69b-13d5676a4b18  
Subcategory: DisasterRecovery

<!--e1967ca0-c0c3-4ae2-b69b-13d5676a4b18_end-->

<!--articleBody-->
