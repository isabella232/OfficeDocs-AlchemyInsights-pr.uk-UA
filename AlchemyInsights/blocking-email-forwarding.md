---
title: Блокування та розблокування зовнішнього автоматичного пересилання електронної пошти
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
ms.openlocfilehash: 6c4ddd53ab794ffad3179dd86a8f81785567cfe34240dff2aa0a1df11094883d
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/11/2021
ms.locfileid: "57897489"
---
# <a name="block-or-unblock-eternal-automatic-email-forwarding"></a>Блокування та розблокування автоматичного пересилання електронної пошти

Щоб дізнатися, як увімкнути або вимкнути пересилання електронної пошти для певної поштової скриньки, див. [цю дія.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

Адміністратори можуть керувати зовнішнім пересиланням для організації за [допомогою політик вихідних спаму.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy) Політики вихідного спаму можна керувати на порталі Microsoft 365 Defender, використовуючи командлет <https://security.microsoft.com/antispam> [Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy) в Exchange Online PowerShell.

Якщо з'являється таке повідомлення про помилку: **"550 5.7.520 Access denied, Your organization does not allow external forwarding" (550 5.7.520 Access denied, Your organization not allow external forwarding" (550 5.7.520 Access відхилено),** переконайтеся, що політику ввімкнуто для зовнішніх автоматично перенаправлених повідомлень.

**Примітка.** Ми рекомендуємо значення за  замовчуванням Автоматично **–** Система керується для параметра Автоматичне пересилання правил у стандартній політиці фільтрування вихідних спаму (автоматичне зовнішнє пересилання заблоковано; все одно працює внутрішнє автоматичне пересилання). Потрібно створити настроювані політики фільтрування вихідних спаму та використовувати значення Увімкнуто **–** Пересилання ввімкнуто лише для користувачів, яким потрібне зовнішнє автоматичне пересилання електронної пошти. Докладні відомості див. [в цій](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)Office 365.
