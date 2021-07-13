---
title: Стан домену – не вибрано жодних служб
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11094"
- "9006491"
ms.openlocfilehash: 66fae5b5602dd67954ac9208b26bc2005adda0e3
ms.sourcegitcommit: 56650eb9af437ff97e4f4d9ca5a2f53ad5bb990e
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/12/2021
ms.locfileid: "53389202"
---
# <a name="domain-status---no-services-selected"></a><span data-ttu-id="3b11f-102">Стан домену – не вибрано жодних служб</span><span class="sxs-lookup"><span data-stu-id="3b11f-102">Domain Status - No services selected</span></span>

<span data-ttu-id="3b11f-103">**Не вибрано жодних** служб означає, що ви не вибрали жодні служби Microsoft 365, як-от Exchange Online, Skype для бізнесу або Intune, а також Керування мобільними пристроями для Microsoft 365 для вашого настроюваного домену.</span><span class="sxs-lookup"><span data-stu-id="3b11f-103">**No services selected** means you haven’t selected any Microsoft 365 services such as Exchange Online, Skype for Business or Intune, and Mobile Device Management for Microsoft 365 to use with your custom domain.</span></span> <span data-ttu-id="3b11f-104">Якщо використовується гібридне середовище Exchange (локальне середовище Exchange із Exchange Online) або зовнішній фільтрування спаму з Exchange без інших служби Microsoft, це повідомлення можна пропустити.</span><span class="sxs-lookup"><span data-stu-id="3b11f-104">If you're using Exchange Hybrid (Exchange on-premises with Exchange Online) or external spam filtering with Exchange and no other Microsoft services, you can ignore this message.</span></span> <span data-ttu-id="3b11f-105">Стан справності домену доступний лише для доменів, підключених безпосередньо до служби.</span><span class="sxs-lookup"><span data-stu-id="3b11f-105">Domain health status is available only for domains connected directly to the service.</span></span>

<span data-ttu-id="3b11f-106">Щоб вибрати служби для домену:</span><span class="sxs-lookup"><span data-stu-id="3b11f-106">To select services for your domain:</span></span>

1. <span data-ttu-id="3b11f-107">У **Настройки** доменів установіть прапорець поруч із доменом, і повідомлення про стан  >  [](https://admin.microsoft.com/Adminportal/Home)Не **вибрано служб.**</span><span class="sxs-lookup"><span data-stu-id="3b11f-107">From **Settings** > [**Domains**](https://admin.microsoft.com/Adminportal/Home), check the box next to the domain with the status message **No services selected**.</span></span>
1. <span data-ttu-id="3b11f-108">Виберіть **Manage DNS (Керування службою DNS),** щоб запустити майстер настроювання домену.</span><span class="sxs-lookup"><span data-stu-id="3b11f-108">Select **Manage DNS** to start the Domain Setup Wizard.</span></span>
    - <span data-ttu-id="3b11f-109">Якщо ви **виберете Додати власні записи DNS,** виберіть службу, коли з'явиться відповідний запит.</span><span class="sxs-lookup"><span data-stu-id="3b11f-109">If you choose **Add your own DNS records**, be sure to select a service when prompted.</span></span> <span data-ttu-id="3b11f-110">Додаткові служби можна знайти в розділі **Додаткові параметри.**</span><span class="sxs-lookup"><span data-stu-id="3b11f-110">More services could be available under **Advanced Options**.</span></span>
    - <span data-ttu-id="3b11f-111">Якщо вибрати дозволити **корпорації Майкрософт додавати ваші записи DNS** або Додаткові параметри Настроювання моїх онлайнових служб, усі доступні служби пропонуються та   >   вибираються автоматично.</span><span class="sxs-lookup"><span data-stu-id="3b11f-111">If you choose **Let Microsoft add your DNS records** or **More options** > **Setup my online services for me** all available services are suggested and selected automatically.</span></span>
1. <span data-ttu-id="3b11f-112">Виконайте всі кроки майстра, щоб завершити настроювання служби DNS і вибрати служби.</span><span class="sxs-lookup"><span data-stu-id="3b11f-112">Continue through the wizard to complete DNS setup and your service choices.</span></span>
 
<span data-ttu-id="3b11f-113">Додаткову довідку з налаштування домену див. в розділі [Додавання записів DNS для підключення домену.](/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)</span><span class="sxs-lookup"><span data-stu-id="3b11f-113">For additional help setting up your domain, see [Add DNS records to connect your domain](/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>

