---
description: "sp_delete_log_shipping_secondary_database (Transact-SQL)"
title: "sp_delete_log_shipping_secondary_database (Transact-SQL) | Microsoft Docs"
ms.custom: ""
ms.date: "03/14/2017"
ms.service: sql
ms.reviewer: ""
ms.subservice: system-objects
ms.topic: "reference"
f1_keywords: 
  - "sp_delete_log_shipping_secondary_database_TSQL"
  - "sp_delete_log_shipping_secondary_database"
dev_langs: 
  - "TSQL"
helpviewer_keywords: 
  - "sp_delete_log_shipping_secondary_database"
ms.assetid: c71b21c0-ec04-4fbd-9735-01128b736935
author: MashaMSFT
ms.author: mathoma
---
# sp_delete_log_shipping_secondary_database (Transact-SQL)
[!INCLUDE [SQL Server](../../includes/applies-to-version/sqlserver.md)]

  This stored procedure removes a secondary database and removes the local history and remote history.  
  
 :::image type="icon" source="../../includes/media/topic-link-icon.svg" border="false"::: [Transact-SQL syntax conventions](../../t-sql/language-elements/transact-sql-syntax-conventions-transact-sql.md)  
  
## Syntax  
  
```  
  
sp_delete_log_shipping_secondary_database  
[ @secondary_database = ] 'secondary_database'  
```  
  
## Arguments  
`[ @secondary_database = ] 'secondary_database'`
 Is the name of the secondary database. *secondary_database* is **sysname**, with no default.  
  
## Return Code Values  
 0 (success) or 1 (failure)  
  
## Result Sets  
 None.  
  
## Remarks  
 **sp_delete_log_shipping_secondary_database** must be run from the **master** database on the secondary server.  
  
## Permissions  
 Only members of the **sysadmin** fixed server role can run this procedure.  
  
## See Also  
 [About Log Shipping &#40;SQL Server&#41;](../../database-engine/log-shipping/about-log-shipping-sql-server.md)   
 [System Stored Procedures &#40;Transact-SQL&#41;](../../relational-databases/system-stored-procedures/system-stored-procedures-transact-sql.md)  
  
  
