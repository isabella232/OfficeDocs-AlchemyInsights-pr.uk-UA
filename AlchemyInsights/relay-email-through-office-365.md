---
title: Ретрансляція електронної пошти через Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 56936541c52e56d7aa9b0f5dad7b9a359c5b6185
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809676"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="a811b-102">Налаштування багатофункціонального пристрою або програми на надсилання електронної пошти</span><span class="sxs-lookup"><span data-stu-id="a811b-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="a811b-103">Відомості про доступні можливості та вказівки див. в статті [Налаштування надсилання повідомлень електронної пошти на багатофункціональному пристрої або в програмі за допомогою Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="a811b-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="a811b-104">**Примітка.** Якщо ви маєте пристрій або програму, які нещодавно перестали працювати, майте на увазі, що останнім часом ми почали [планове вимкнення шифрування 3DES](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption).</span><span class="sxs-lookup"><span data-stu-id="a811b-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="a811b-105">Щоб побачити вражені пристрої, перейдіть до [Звіту клієнтів з автентифікації SMTP](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="a811b-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="a811b-106">Серед типових помилок можуть бути: помилка автентифікації, помилка TLS, помилка алгоритму шифрування, невідповідність алгоритму або розрив підключення.</span><span class="sxs-lookup"><span data-stu-id="a811b-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="a811b-107">Вирішення проблеми:</span><span class="sxs-lookup"><span data-stu-id="a811b-107">To resolve the issue:</span></span>

 - <span data-ttu-id="a811b-108">**Windows Server 2003 IIS SMTP більше не підтримується – потрібна новіша версія операційної системи.**</span><span class="sxs-lookup"><span data-stu-id="a811b-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="a811b-109">З'ясуйте у постачальника вашої програми або пристрою, чи підтримується сучасне шифрування або чи є оновлення.</span><span class="sxs-lookup"><span data-stu-id="a811b-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
