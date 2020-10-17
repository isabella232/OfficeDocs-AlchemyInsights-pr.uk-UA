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
ms.openlocfilehash: 2f3528375d251542fd82761d00c776706de2e23c
ms.sourcegitcommit: f7b82f75a5400e992ecbd48a666783354e2e2871
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/15/2020
ms.locfileid: "48473122"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="f438b-102">Блокування та розблокування пересилання електронної пошти</span><span class="sxs-lookup"><span data-stu-id="f438b-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="f438b-103">Щоб увімкнути або вимкнути пересилання електронної пошти для певної поштової скриньки, перегляньте статтю [настроювання пересилання електронної пошти](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="f438b-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="f438b-104">На рівні клієнта керування зовнішньою експедицією здійснюється за допомогою вихідної політики спаму.</span><span class="sxs-lookup"><span data-stu-id="f438b-104">On the tenant level, control of external forwarding is done using the outbound spam policy.</span></span> <span data-ttu-id="f438b-105">Ви можете перевірити політику фільтра вихідної небажаної пошти в центрі безпеки та відповідності [тут] ( https://protection.office.com/antispam) або за допомогою [команди Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span><span class="sxs-lookup"><span data-stu-id="f438b-105">You can check the outbound spam filter policy from Security and Compliance Center [here] (https://protection.office.com/antispam) or by using the [Get-HostedOutboundSpamFilterPolicy command](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span></span>

<span data-ttu-id="f438b-106">Якщо з'являється таке повідомлення про помилку: **"550" відмовлено в доступі, ваша організація не підтримує зовнішню переадресацію "**, переконайтеся, що цю політику настроєно для ввімкнення зовнішнього автоматичного пересилання.</span><span class="sxs-lookup"><span data-stu-id="f438b-106">If you are getting the following error: **“550 5.7.520 Access denied, Your organization does not allow external forwarding”**, please make sure the policy is configured to enable External Auto-forward.</span></span>

<span data-ttu-id="f438b-107">**Примітка.** Рекомендується зберегти зовнішній Автопересилання, вимкнутий у політиці вихідної пошти за замовчуванням, і активувати його лише для користувачів, яким потрібна зовнішня переадресація, створивши настроювану політику для цих користувачів.</span><span class="sxs-lookup"><span data-stu-id="f438b-107">**Note:** It is recommended to keep the External Autoforward disabled on your default outbound spam filter policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="f438b-108">Ви можете дізнатися більше про те, як [настроювати зовнішні пересилання електронної пошти в Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="f438b-108">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>