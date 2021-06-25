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
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>Налаштування багатофункціонального пристрою або програми на надсилання електронної пошти

Відомості про доступні можливості та вказівки див. в статті [Налаштування надсилання повідомлень електронної пошти на багатофункціональному пристрої або в програмі за допомогою Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).
  
Якщо у вас пристрій або програма, які нещодавно припинили роботу, найпоширеніші з них:

- **Помилки, пов'язані з автентифікацією під** час використання надсилання через клієнт SMTP Auth Нещодавно ми внесли деякі зміни, пов'язані з автентифікацією SMTP. Докладні відомості про вирішення проблем див. в розділі Невдала автентифікація у статті Вирішення проблем із принтерами, сканерами та бізнес-програмами, які надсилують повідомлення електронної пошти за допомогою [Microsoft 365 або Office 365.](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)
- **Ми приймаємо лише версію TLS 1.2, роблячи безпечне** підключення Office 365 Якщо використовується безпечне підключення (TLS), переконайтеся, що ваш пристрій програми підтримує протокол TLS 1.2. Докладні відомості див. в Office 365 та [Office 365 GCC TLS 1.2.](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)
 
Інші проблеми та вирішення див. в розділі Вирішення проблем із принтерами, сканерами та бізнес-програмами, які надсилайте електронні листи за [допомогою Microsoft 365 або Office 365.](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)

Щоб побачити вражені пристрої, перейдіть до [Звіту клієнтів з автентифікації SMTP](https://protection.office.com/mailflow/dashboard).

**Примітка.** Exchange Online сценарії групової розсилки не можна. Щоб надіслати групову комерційну електронну пошту (наприклад, бюлетень клієнтів), використовуйте сторонніх постачальників, які спеціалізуються на цих службах.
