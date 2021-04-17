---
title: Власник не може створити вкладену папку за допомогою Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836156"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="57b8f-102">Власник не може створити вкладену папку за допомогою Outlook</span><span class="sxs-lookup"><span data-stu-id="57b8f-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="57b8f-103">**Власники спільних папок, які створюють вкладені папки за допомогою Outlook, можуть виникати незмінні проблеми. Цю проблему буде вирішено незабаром.**</span><span class="sxs-lookup"><span data-stu-id="57b8f-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="57b8f-104">Тим часом скористайтеся одним із наведених нижче способів вирішення.</span><span class="sxs-lookup"><span data-stu-id="57b8f-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="57b8f-105">Створення вкладеної папки в Outlook для Mac, оскільки ця проблема виникає лише в Outlook для настільних комп'ютерів (усі версії)</span><span class="sxs-lookup"><span data-stu-id="57b8f-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="57b8f-106">Адміністратор може створити вкладену адресу за допомогою EXO Shell або EAC</span><span class="sxs-lookup"><span data-stu-id="57b8f-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="57b8f-107">Змінення параметра DefaultPublicFolderMailbox/EffectivePublicFolderMailbox користувача на іншу поштову скриньку, відмінну від поштової скриньки вмісту папки, яка виникає, коли проблема виникає</span><span class="sxs-lookup"><span data-stu-id="57b8f-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="57b8f-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="57b8f-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="57b8f-109">Зачекайте годину, перезапустіть клієнт Outlook</span><span class="sxs-lookup"><span data-stu-id="57b8f-109">Wait for an hour, restart outlook client</span></span>