---
title: Встановити або змінити дозволи спільної папки
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 8/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: d1554e8a63455f3549044e526183c0e8709f2631
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/22/2019
ms.locfileid: "30767305"
---
# <a name="permissions-and-public-folders"></a>Дозволи та спільних папок

Ви можете змінити дозволи на спільних папок за допомогою Outlook, адміністратор Exchange центр (EAC), або PowerShell:
  
- Докладніше Outlook, [натисніть тут](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).
    
- EAC можна знайти перегляньте [цю статтю](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) . Натисніть [тут](https://support.office.com/article/ https://outlook.office365.com/ecp/.aspx) для переходу до EAC. 
    
- Powershell можна знайти перегляньте [цю статтю](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) про використання commandlet Add-PublicFolderClientPermission. Якщо вам потрібні інструкції для підключення до Exchange Powershell, натисніть [тут](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).
    
Якщо **зовнішні користувачі не можуть відправляти електронну пошту до спільної папки пошти**, причина може бути що спільної папки відсутні дозволи необхідні для доставки електронної пошти зовнішніх. Це можна виправити за допомогою Outlook інструкції [тут](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), або PowerShell інструкції [тут](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).
  

