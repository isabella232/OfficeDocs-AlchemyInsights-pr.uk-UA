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
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/24/2021
ms.locfileid: "53118004"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="7cb05-102">Налаштування багатофункціонального пристрою або програми на надсилання електронної пошти</span><span class="sxs-lookup"><span data-stu-id="7cb05-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="7cb05-103">Відомості про доступні можливості та вказівки див. в статті [Налаштування надсилання повідомлень електронної пошти на багатофункціональному пристрої або в програмі за допомогою Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="7cb05-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="7cb05-104">Якщо у вас пристрій або програма, які нещодавно припинили роботу, найпоширеніші з них:</span><span class="sxs-lookup"><span data-stu-id="7cb05-104">If you have a device or application that recently stopped working, the most common issues are:</span></span>

- <span data-ttu-id="7cb05-105">**Помилки, пов'язані з автентифікацією під** час використання надсилання через клієнт SMTP Auth Нещодавно ми внесли деякі зміни, пов'язані з автентифікацією SMTP.</span><span class="sxs-lookup"><span data-stu-id="7cb05-105">**Authentication related errors while using SMTP Auth client submission** We recently made some changes related to how SMTP Authentication works.</span></span> <span data-ttu-id="7cb05-106">Докладні відомості про вирішення проблем див. в розділі Невдала автентифікація у статті Вирішення проблем із принтерами, сканерами та бізнес-програмами, які надсилують повідомлення електронної пошти за допомогою [Microsoft 365 або Office 365.](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)</span><span class="sxs-lookup"><span data-stu-id="7cb05-106">For more information about how to resolve issues, see the authentication unsuccessful section of [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).</span></span>
- <span data-ttu-id="7cb05-107">**Ми приймаємо лише версію TLS 1.2, роблячи безпечне** підключення Office 365 Якщо використовується безпечне підключення (TLS), переконайтеся, що ваш пристрій програми підтримує протокол TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="7cb05-107">**We accept only the TLS 1.2 version while making a secure connection to Office 365** If you're using Secure connection (TLS), make sure your application device supports TLS 1.2.</span></span> <span data-ttu-id="7cb05-108">Докладні відомості див. в Office 365 та [Office 365 GCC TLS 1.2.](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="7cb05-108">For more information, see [Preparing for TLS 1.2 in Office 365 and Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span></span>
 
<span data-ttu-id="7cb05-109">Інші проблеми та вирішення див. в розділі Вирішення проблем із принтерами, сканерами та бізнес-програмами, які надсилайте електронні листи за [допомогою Microsoft 365 або Office 365.](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)</span><span class="sxs-lookup"><span data-stu-id="7cb05-109">For other issues and solutions, see [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).</span></span>

<span data-ttu-id="7cb05-110">Щоб побачити вражені пристрої, перейдіть до [Звіту клієнтів з автентифікації SMTP](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="7cb05-110">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span>

<span data-ttu-id="7cb05-111">**Примітка.** Exchange Online сценарії групової розсилки не можна.</span><span class="sxs-lookup"><span data-stu-id="7cb05-111">**Note**: Exchange Online doesn't accommodate bulk-mailing scenarios.</span></span> <span data-ttu-id="7cb05-112">Щоб надіслати групову комерційну електронну пошту (наприклад, бюлетень клієнтів), використовуйте сторонніх постачальників, які спеціалізуються на цих службах.</span><span class="sxs-lookup"><span data-stu-id="7cb05-112">To send bulk commercial email (for example, customer newsletters), you should use third-party providers that specialize in these services.</span></span>
