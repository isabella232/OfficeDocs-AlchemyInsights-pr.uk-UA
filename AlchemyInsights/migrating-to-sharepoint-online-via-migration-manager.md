---
title: Перенесення до SharePoint Online за допомогою диспетчера міграції
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3192"
ms.openlocfilehash: 5aebf7903670e74f616c8f151749d760caf1d642
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932377"
---
# <a name="migrating-to-sharepoint-online-via-migration-manager"></a><span data-ttu-id="d9180-102">Перенесення до SharePoint Online за допомогою диспетчера міграції</span><span class="sxs-lookup"><span data-stu-id="d9180-102">Migrating to SharePoint Online via Migration Manager</span></span>

<span data-ttu-id="d9180-103">**Важливо**. Багато клієнтів SharePoint Online і OneDrive запускають у службі критично важливі для бізнесу програми, що працюють у фоновому режимі.</span><span class="sxs-lookup"><span data-stu-id="d9180-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="d9180-104">До них належать перенесення вмісту, захист від втрати даних (DLP) та рішення для резервного копіювання.</span><span class="sxs-lookup"><span data-stu-id="d9180-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="d9180-105">У цей безпрецедентний час ми працюємо над тим, щоб служби SharePoint Online і OneDrive залишалися високодоступними та надійними для користувачів, які залежать від них більше, ніж будь-коли, через віддалену роботу.</span><span class="sxs-lookup"><span data-stu-id="d9180-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="d9180-106">З цією метою ми впровадили жорсткіші обмеження кількості запитів для фонових програм (перенесення, DLP та рішення для резервного копіювання) у денний час у будні дні.</span><span class="sxs-lookup"><span data-stu-id="d9180-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="d9180-107">Слід очікувати, що пропускну здатність цих програм буде дуже сильно обмежено протягом цього часу.</span><span class="sxs-lookup"><span data-stu-id="d9180-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="d9180-108">Проте у вечірній час та по вихідних (для конкретного регіону) служба зможе обробляти значно більший обсяг запитів від фонових програм.</span><span class="sxs-lookup"><span data-stu-id="d9180-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="d9180-109">**Диспетчер міграції**</span><span class="sxs-lookup"><span data-stu-id="d9180-109">**Migration Manager**</span></span>

<span data-ttu-id="d9180-110">Диспетчер міграції, розташований у сучасному Центрі адміністрування SharePoint, допоможе вам настроїти клієнти та створити завдання.</span><span class="sxs-lookup"><span data-stu-id="d9180-110">Located in the modern SharePoint Admin Center, the Migration Manager guides you through the setup of your clients and the creation of your tasks.</span></span> <span data-ttu-id="d9180-111">Ви можете вказати глобальні параметри або параметри на рівні завдання, переглянути перебіг виконання всіх завдань, а також завантажити зведення та звіти на рівні завдань.</span><span class="sxs-lookup"><span data-stu-id="d9180-111">You can specify global or task-level settings, view all-up task progress, and download aggregated summary and task-level reports.</span></span>

- [<span data-ttu-id="d9180-112">Початок роботи з диспетчером міграції</span><span class="sxs-lookup"><span data-stu-id="d9180-112">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="d9180-113">Налаштування клієнтів диспетчера міграції</span><span class="sxs-lookup"><span data-stu-id="d9180-113">Setup Migration Manager clients</span></span>](https://docs.microsoft.com/sharepointmigration/mm-setup-clients)

- [<span data-ttu-id="d9180-114">Параметри диспетчера міграції</span><span class="sxs-lookup"><span data-stu-id="d9180-114">Migration Manager Settings</span></span>](https://docs.microsoft.com/sharepointmigration/mm-settings)
