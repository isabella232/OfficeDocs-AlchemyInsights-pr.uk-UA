---
title: 726 блокує пересилання електронної пошти
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
ms.openlocfilehash: 610013c4f46e999f1a8715aea14dd557ed8b0e2a
ms.sourcegitcommit: 88f24bb6ced16842de165af416e3f21feae13063
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/15/2020
ms.locfileid: "48478318"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Блокування та розблокування пересилання електронної пошти

Щоб увімкнути або вимкнути пересилання електронної пошти для певної поштової скриньки, перегляньте статтю [настроювання пересилання електронної пошти](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

На рівні клієнта керування зовнішньою експедицією здійснюється за допомогою вихідної політики спаму. Ви можете перевірити політику фільтра вихідної небажаної пошти в центрі безпеки та відповідності [, а також](https://protection.office.com/antispam) за допомогою [команди Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).

Якщо з'являється таке повідомлення про помилку: **"550" відмовлено в доступі, ваша організація не підтримує зовнішню переадресацію "**, переконайтеся, що цю політику настроєно для ввімкнення зовнішнього автоматичного пересилання.

**Примітка.** Рекомендується зберегти зовнішній Автопересилання, вимкнутий у політиці вихідної пошти за замовчуванням, і активувати його лише для користувачів, яким потрібна зовнішня переадресація, створивши настроювану політику для цих користувачів. Ви можете дізнатися більше про те, як [настроювати зовнішні пересилання електронної пошти в Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).