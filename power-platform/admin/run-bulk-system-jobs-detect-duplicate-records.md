---
title: "Run bulk system jobs to detect duplicate records  | MicrosoftDocs"
description: Run bulk system jobs to detect duplicate records
author: jimholtz
manager: kvivek
ms.service: power-platform
ms.component: pa-admin
ms.topic: conceptual
ms.date: 09/30/2017
ms.author: jimholtz
search.audienceType: 
  - admin
search.app: 
  - D365CE
  - PowerApps
  - Powerplatform
---
# Run bulk system jobs to detect duplicate records

[!INCLUDE [cc-settings-moving](../includes/cc-settings-moving.md)] 

To maintain the integrity of system data, you should check for duplicates regularly to make sure that users don’t inadvertently create duplicate contacts, accounts, leads, or other types of records.  
  
 The Check for Duplicates wizard helps you set up a bulk “job” that finds and cleans up duplicate records. You can schedule the job to run daily, and you can receive an email confirmation when the job finishes.  
  
> [!NOTE]
>  If you haven’t already done so, create and publish duplicate detection rules, and turn duplicate detection on before you run the wizard. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [Set up duplicate detection rules to keep your data clean](../admin/set-up-duplicate-detection-rules-keep-data-clean.md)  
  
1. [!INCLUDE[proc_settings_datamanagement](../includes/proc-settings-datamanagement.md)]  
  
2. Click **Duplicate Detection Jobs**.  
  
3. Click **New**, or select the name of the duplicate detection job you want to run.  
  
    You’ll see the Duplicate Detection wizard, which helps you create a job to check for duplicates.  
  
4. Click **Next**.  
  
5. In the **Look for** drop-down list, select the record type that you want to check for duplicates.  
  
   > [!NOTE]
   >  What you see in this list depends on which duplicate detection rules are published. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [Set up duplicate detection rules to keep your data clean](../admin/set-up-duplicate-detection-rules-keep-data-clean.md)  
  
6. In the **Use Saved View** drop-down list, select a view if you want to limit the records searched to records in that view. For example, select Active Accounts. When you select a view, model-driven apps in Dynamics 365, such as Dynamics 365 Sales and Customer Service, add the criteria to search on.  
  
7. To further limit the records searched, click **Select** and then enter the criteria you want.  
  
   ![Screenshot of duplicate detection wizard, page 1](../admin/media/duplicate-detection-wizard.png "Screenshot of duplicate detection wizard, page 1")  
  
8. Click **Next**.  
  
9. Accept the default name for the job, or type a different name.  
  
10. Enter the start time for the job, and enter how often to run the job in days. (To run the job daily, type `1`.)  
  
11. If you want to receive an email confirmation when the job is completed, select the **Email options** check box. Enter an additional email address, if desired.  
  
12. Click **Next**, and then click **Submit**.  
  
### See also  
 [Set up duplicate detection rules to keep your data clean](../admin/set-up-duplicate-detection-rules-keep-data-clean.md)   
 [Turn duplicate detection rules on or off for the whole organization](../admin/turn-duplicate-detection-rules-off-whole-organization.md)   
 [View and take action on bulk deletion jobs](../admin/view-take-action-bulk-deletion-jobs.md)   
 [Detect duplicate data](detect-duplicate-data.md)
