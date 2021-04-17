---
title: Керування ними
ms.author: pebaum
author: pebaum
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1556"
- "9000080"
ms.openlocfilehash: c7dc35a484894e147208ef7080c151c6d3af0c63
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817733"
---
# <a name="co-management"></a><span data-ttu-id="35918-102">Керування ними</span><span class="sxs-lookup"><span data-stu-id="35918-102">Co-management</span></span>

<span data-ttu-id="35918-103">**Передумови для перенесення з гібридного диспетчера конфігурації до Intune**</span><span class="sxs-lookup"><span data-stu-id="35918-103">**Prerequisites for migrating from Config Manager Hybrid to Intune**</span></span>

- <span data-ttu-id="35918-104">Перегляньте [цю статтю.](https://docs.microsoft.com/mem/configmgr/mdm/understand/what-happened-to-hybrid)</span><span class="sxs-lookup"><span data-stu-id="35918-104">Review [this article](https://docs.microsoft.com/mem/configmgr/mdm/understand/what-happened-to-hybrid).</span></span>
- <span data-ttu-id="35918-105">[Додайте ліцензію Intune для користувачів.](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign)</span><span class="sxs-lookup"><span data-stu-id="35918-105">[Add an Intune license to your users](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign).</span></span>
- <span data-ttu-id="35918-106">[Налаштовуйте](https://www.microsoft.com/edge) співавтентичне керування в Edge за допомогою браузера.</span><span class="sxs-lookup"><span data-stu-id="35918-106">Use the [Edge browser](https://www.microsoft.com/edge) when configuring Co-management.</span></span>

<span data-ttu-id="35918-107">Покрокові вказівки з настроювання співкерування див. [тут.](https://admin.microsoft.com/AdminPortal/Home?#/modernonboarding/comanagesetupguide)</span><span class="sxs-lookup"><span data-stu-id="35918-107">A guided, step-by-step Co-management setup experience can be found [here](https://admin.microsoft.com/AdminPortal/Home?#/modernonboarding/comanagesetupguide).</span></span>

<span data-ttu-id="35918-108">**Інсталяція клієнта Config Manager на пристроях, керованих Intune**</span><span class="sxs-lookup"><span data-stu-id="35918-108">**How to I install the Config Manager client on Intune-managed devices**</span></span>

<span data-ttu-id="35918-109">Докладні відомості див. в розділі Пристрої [з Windows, що керовані MDM в Intune.](https://docs.microsoft.com/mem/configmgr/core/clients/deploy/deploy-clients-to-windows-computers#bkmk_mdm)</span><span class="sxs-lookup"><span data-stu-id="35918-109">See [Intune MDM-managed Windows devices](https://docs.microsoft.com/mem/configmgr/core/clients/deploy/deploy-clients-to-windows-computers#bkmk_mdm).</span></span>

<span data-ttu-id="35918-110">**Що робити, якщо потрібно просто змінити повноваження MDM?**</span><span class="sxs-lookup"><span data-stu-id="35918-110">**What if I just want to change MDM authority?**</span></span>

<span data-ttu-id="35918-111">MDM Authority можна змінити, не відкриваючи інцидент служби підтримки.</span><span class="sxs-lookup"><span data-stu-id="35918-111">MDM Authority can be changed without opening a support case.</span></span> <span data-ttu-id="35918-112">Перегляньте наведену нижче документацію, щоб допомогти у зміні списку дозволів MDM:</span><span class="sxs-lookup"><span data-stu-id="35918-112">Please review the following documentation to assist in changing your MDM authority:</span></span>

- [<span data-ttu-id="35918-113">Змініть MDM Authority з Configuration Manager (Диспетчер конфігурацій) на Автономний режим Intune</span><span class="sxs-lookup"><span data-stu-id="35918-113">Change MDM Authority from Configuration Manager to Intune standalone</span></span>](https://docs.microsoft.com/mem/configmgr/mdm/understand/what-happened-to-hybrid)
- [<span data-ttu-id="35918-114">Змінення автономної системи MDM з автономної системи Intune на Диспетчер конфігурацій</span><span class="sxs-lookup"><span data-stu-id="35918-114">Change MDM authority from Intune standalone to Configuration Manager</span></span>](https://docs.microsoft.com/mem/configmgr/mdm/understand/what-happened-to-hybrid)
