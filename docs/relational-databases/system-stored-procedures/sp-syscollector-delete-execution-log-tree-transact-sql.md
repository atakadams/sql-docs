---
description: "sp_syscollector_delete_execution_log_tree (Transact-SQL)"
title: "sp_syscollector_delete_execution_log_tree (Transact-SQL) | Microsoft Docs"
ms.custom: ""
ms.date: "03/14/2017"
ms.service: sql
ms.reviewer: ""
ms.subservice: system-objects
ms.topic: "reference"
f1_keywords: 
  - "sp_syscollector_delete_execution_log_tree_TSQL"
  - "sp_syscollector_delete_execution_log_tree"
dev_langs: 
  - "TSQL"
helpviewer_keywords: 
  - "sp_syscollector_delete_execution_log_tree"
  - "data collector [SQL Server], stored procedures"
ms.assetid: 0a9a7c5b-c3cc-40ca-b524-e948a8cce4e4
author: markingmyname
ms.author: maghan
---
# sp_syscollector_delete_execution_log_tree (Transact-SQL)
[!INCLUDE [SQL Server](../../includes/applies-to-version/sqlserver.md)]

  Deletes all the log entries for the run of a single collection set. It also deletes the log entries from the [!INCLUDE[ssIS](../../includes/ssis-md.md)] tables for that run.  
  
 :::image type="icon" source="../../includes/media/topic-link-icon.svg" border="false"::: [Transact-SQL syntax conventions](../../t-sql/language-elements/transact-sql-syntax-conventions-transact-sql.md)  
  
## Syntax  
  
```  
  
sp_syscollector_delete_execution_log_tree[ @log_id = ] log_id  
          , [ @from_collection_set = ] from_collection_set  
```  
  
## Arguments  
`[ @log_id = ] log_id`
 Is the unique identifier for the collection set log. *log_id* is **int**.  
  
`[ @from_collection_set = ] from_collection_set`
 Is the identifier for the collection set. *from_collection_set* is **bit=1**.  
  
## Return Code Values  
 **0** (success) or **1** (failure)  
  
## Permissions  
 Requires membership in the **dc_operator** (with EXECUTE permission) fixed database role to execute this procedure.  
  
## See Also  
 [System Stored Procedures &#40;Transact-SQL&#41;](../../relational-databases/system-stored-procedures/system-stored-procedures-transact-sql.md)  
  
  
