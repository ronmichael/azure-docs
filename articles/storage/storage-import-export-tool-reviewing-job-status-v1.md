---
title: Reviewing Job Status with Copy Log Files | Microsoft Docs
description: Learn how to use the log files created when the import or export job was run to see the status of the Import-Export Job. 
author: muralikk
manager: syadav
editor: tysonn
services: storage
documentationcenter: ''

ms.assetid: c69d1d69-6403-4eee-9949-0185faeecfa1
ms.service: storage
ms.workload: storage 
ms.tgt_pltfrm: na
ms.devlang: na
ms.topic: article
ms.date: 01/26/2017
ms.author: muralikk

---

# Reviewing Job Status with Copy Log Files
When the Microsoft Azure Import/Export service processes drives associated with an import or export job, it writes copy log files to the storage account to or from which you are importing or exporting blobs. The log file contains detailed status about each file that was imported or exported. The URL to each copy log file is returned when you query the status of a completed job; see [Get Job](/rest/api/storageservices`Get-Job3) for more information.  
  
 The following are example URLs for copy log files for an import job with two drives:  
  
 `http://myaccount.blob.core.windows.net/ImportExportStatesPath/waies/myjob_9WM35C2V_20130921-034307-902_error.xml`  
  
 `http://myaccount.blob.core.windows.net/ImportExportStatesPath /waies/myjob_9WM45A6Q_20130921-042122-021_error.xml`  
  
 See [Import-Export Service Log File Format](storage-import-export-file-format-log.md) for the format of copy logs and the full list of status codes.  
  
## See Also  
 [Setting Up the Azure Import-Export Tool](storage-import-export-tool-setup-v1.md)   
 [Preparing Hard Drives for an Import Job](storage-import-export-tool-preparing-hard-drives-import-v1.md)   
 [Repairing an Import Job](storage-import-export-tool-repairing-an-import-job-v1.md)   
 [Repairing an Export Job](storage-import-export-tool-repairing-an-export-job-v1.md)   
 [Troubleshooting the Azure Import-Export Tool](storage-import-export-tool-troubleshooting-v1.md)
