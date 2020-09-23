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
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219876"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="bc154-102">Блокування та розблокування пересилання електронної пошти</span><span class="sxs-lookup"><span data-stu-id="bc154-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="bc154-103">Щоб увімкнути або вимкнути пересилання електронної пошти для певної поштової скриньки, перегляньте статтю [настроювання пересилання електронної пошти](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="bc154-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="bc154-104">На рівні клієнта контроль за зовнішнім експедитором здійснюється за допомогою вихідної політики захисту від спаму.</span><span class="sxs-lookup"><span data-stu-id="bc154-104">On the tenant level, control of External forwarding is done using the outbound anti-spam policy.</span></span> <span data-ttu-id="bc154-105">Якщо його настроєно на вимкнення або автоматичне, це може блокувати пересилання електронної пошти за допомогою "550 5.7.520 Access відмовлено, ваша організація не дозволяє зовнішню переадресацію".</span><span class="sxs-lookup"><span data-stu-id="bc154-105">If it is set to Off or Automatic, it might block email forwarding with the “550 5.7.520 Access denied, Your organization does not allow external forwarding” error.</span></span> <span data-ttu-id="bc154-106">Згодом, якщо було настроєно переадресацію, це повідомлення про помилку бачитимуть користувачі.</span><span class="sxs-lookup"><span data-stu-id="bc154-106">Subsequently, if forwarding was set to be blocked, that is the error your users will see.</span></span>

<span data-ttu-id="bc154-107">Якщо пересилання буде заблоковано, переконайтеся, що політику настроєно для ввімкнення зовнішнього автоматичного пересилання.</span><span class="sxs-lookup"><span data-stu-id="bc154-107">If forwarding is being blocked, please make sure the policy is configured to enable External Autoforward.</span></span> <span data-ttu-id="bc154-108">Ви можете перевірити політику фільтра вихідної небажаної пошти в центрі безпеки та відповідності або запустивши команду Get-HostedOutboundSpamFilterPolicy | ім'я FL, режим автоматичного переадресації.</span><span class="sxs-lookup"><span data-stu-id="bc154-108">You can check the Outbound Spam Filter Policy from Security and Compliance Center or by running command Get-HostedOutboundSpamFilterPolicy | fl name,AutoForwardingMode.</span></span> <span data-ttu-id="bc154-109">Якщо потрібно настроїти блокування автоматичного пересилання, ця команда розповість про стан політики зараз.</span><span class="sxs-lookup"><span data-stu-id="bc154-109">If you want to set up Autoforward blocking, the same command will tell you the state of policy now.</span></span>

<span data-ttu-id="bc154-110">Примітка: рекомендується зберігати зовнішній Автопересилання, вимкнуту в політиці "вихідний спам" за замовчуванням, і активувати його лише для користувачів, яким потрібна зовнішня переадресація, створивши настроювану політику для цих користувачів.</span><span class="sxs-lookup"><span data-stu-id="bc154-110">Note: It is recommended to keep the External Autoforward disabled on your Default Outbound Spam Filter Policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="bc154-111">Ви можете дізнатися більше про те, як [настроювати зовнішні пересилання електронної пошти в Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="bc154-111">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>