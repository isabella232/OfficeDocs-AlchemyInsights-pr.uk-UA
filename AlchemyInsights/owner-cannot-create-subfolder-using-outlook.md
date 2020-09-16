---
title: Власник не може створювати вкладену папку за допомогою програми Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665739"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="1e1a5-102">Власник не може створювати вкладену папку за допомогою програми Outlook</span><span class="sxs-lookup"><span data-stu-id="1e1a5-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="1e1a5-103">**Виникла проблема з власниками спільних папок, що створюють вкладені папки за допомогою програми Outlook. Ця проблема буде усунена найближчим часом.**</span><span class="sxs-lookup"><span data-stu-id="1e1a5-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="1e1a5-104">Тим часом, скористайтеся одним із наведених нижче способів вирішення.</span><span class="sxs-lookup"><span data-stu-id="1e1a5-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="1e1a5-105">Використання програми Outlook для MAC для створення вкладеної папки як засобу впливає лише на програму Outlook для настільних комп'ютерів (усі версії)</span><span class="sxs-lookup"><span data-stu-id="1e1a5-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="1e1a5-106">Адміністратор створює вкладену папку за допомогою оболонки EXO або EAC</span><span class="sxs-lookup"><span data-stu-id="1e1a5-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="1e1a5-107">Змінення за промовчанням поштової скриньки або ефективності поштової скриньки користувача в іншій поштовій скриньці, ніж у поштовій скриньці вмісту для папки, яка викликає помилку</span><span class="sxs-lookup"><span data-stu-id="1e1a5-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="1e1a5-108">*Настроювання – поштова скринька User1 Def"поштова скринька" PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="1e1a5-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="1e1a5-109">Зачекайте години, перезапустіть клієнт Outlook</span><span class="sxs-lookup"><span data-stu-id="1e1a5-109">Wait for an hour, restart outlook client</span></span>