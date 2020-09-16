---
title: Установлення або змінення дозволів для спільної папки
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: c035d56ffade45cc4360a1d0dfca4c63bf110a38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771211"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="31945-102">Дозволи та спільні папки</span><span class="sxs-lookup"><span data-stu-id="31945-102">Permissions and Public Folders</span></span>

<span data-ttu-id="31945-103">Ви можете змінити дозволи для спільних папок за допомогою програми Outlook, центру адміністрування Exchange (EAC) або PowerShell:</span><span class="sxs-lookup"><span data-stu-id="31945-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="31945-104">Щоб отримати вказівки з Outlook, [клацніть тут](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span><span class="sxs-lookup"><span data-stu-id="31945-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="31945-105">У [цій статті](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) наведено вказівки з указівок для EAC.</span><span class="sxs-lookup"><span data-stu-id="31945-105">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions.</span></span> 
    
- <span data-ttu-id="31945-106">У PowerShell, зверніться до [цієї статті](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) , щоб отримати вказівки з використання надбудови чином.</span><span class="sxs-lookup"><span data-stu-id="31945-106">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet.</span></span> <span data-ttu-id="31945-107">Якщо вам потрібні інструкції для підключення до Exchange PowerShell, клацніть [тут](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span><span class="sxs-lookup"><span data-stu-id="31945-107">If you need instructions to connect to Exchange Powershell, click [here](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="31945-108">Якщо **зовнішні користувачі не можуть надсилати повідомлення електронної пошти до спільної папки з підтримкою пошти**, причиною може бути те, що спільна папка не містить дозволів, потрібних для зовнішньої доставки електронної пошти.</span><span class="sxs-lookup"><span data-stu-id="31945-108">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery.</span></span> <span data-ttu-id="31945-109">Цю проблему можна вирішити за [допомогою інструкцій](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx)програми [Outlook, а також інструкцій PowerShell](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1).</span><span class="sxs-lookup"><span data-stu-id="31945-109">You can fix this using the Outlook instructions [here](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

