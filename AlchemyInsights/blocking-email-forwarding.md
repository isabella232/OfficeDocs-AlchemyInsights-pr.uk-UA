---
title: Блокування пересилання електронної пошти (726)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: 0bff7ede02809e133dc6616452ec840f552bd4fa6c45b7987d6455b2a9ba49bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059653"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Блокування або розблокування пересилання електронної пошти

Щоб дізнатися, як увімкнути або вимкнути пересилання електронної пошти для певної поштової скриньки, див. [цю дія.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

Керування зовнішнім пересиланням на рівні клієнта здійснюється за допомогою політики вихідного спаму. Політику фільтрування вихідних спамів можна [](https://protection.office.com/antispam) переглянути в Центрі безпеки та відповідності тут або за допомогою команди [Get-HostedOutboundSpamFilterPolicy.](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy)

Якщо з'являється таке повідомлення про помилку: **"550 5.7.520 Access denied, Your organization does not allow external forwarding" (550 5.7.520 Access відхилено),** переконайтеся, що в організації не дозволено пересилання зовнішніх користувачів.

**Примітка.** Ми рекомендуємо не вимикати функцію "Зовнішній автофільтр" у стандартній політиці фільтрування вихідних спаму та ввімкнути її лише для користувачів, яким потрібне зовнішнє пересилання, створивши спеціальну політику для цих користувачів. Докладні відомості див. в [Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)в цій Office 365.