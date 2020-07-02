---
title: Ретрансляція електронної пошти через Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 074a9106553bf3a2a5e563f9ebaca9dfc38111cb
ms.sourcegitcommit: 9872280f71429d2344b0b441e218fba5b3bd3cf7
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/02/2020
ms.locfileid: "45023480"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="5f0c7-102">Налаштування багатофункціонального пристрою або програми на надсилання електронної пошти</span><span class="sxs-lookup"><span data-stu-id="5f0c7-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="5f0c7-103">Відомості про доступні можливості та вказівки див. в статті [Налаштування надсилання повідомлень електронної пошти на багатофункціональному пристрої або в програмі за допомогою Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="5f0c7-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="5f0c7-104">**Примітка.** Якщо ви маєте пристрій або програму, які нещодавно перестали працювати, майте на увазі, що останнім часом ми почали [планове вимкнення шифрування 3DES](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption).</span><span class="sxs-lookup"><span data-stu-id="5f0c7-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="5f0c7-105">Щоб побачити вражені пристрої, перейдіть до [Звіту клієнтів з автентифікації SMTP](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="5f0c7-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="5f0c7-106">Серед типових помилок можуть бути: помилка автентифікації, помилка TLS, помилка алгоритму шифрування, невідповідність алгоритму або розрив підключення.</span><span class="sxs-lookup"><span data-stu-id="5f0c7-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="5f0c7-107">Вирішення проблеми:</span><span class="sxs-lookup"><span data-stu-id="5f0c7-107">To resolve the issue:</span></span>

 - <span data-ttu-id="5f0c7-108">**Windows Server 2003 IIS SMTP більше не підтримується – потрібна новіша версія операційної системи.**</span><span class="sxs-lookup"><span data-stu-id="5f0c7-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="5f0c7-109">З'ясуйте у постачальника вашої програми або пристрою, чи підтримується сучасне шифрування або чи є оновлення.</span><span class="sxs-lookup"><span data-stu-id="5f0c7-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
