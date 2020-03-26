---
title: Загальні вказівки з ефективності перенесення
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
- "3179"
ms.openlocfilehash: 10a0069c41d2e5128b2592425d815364a83b730f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932499"
---
# <a name="general-migration-performance-guidance"></a><span data-ttu-id="f0015-102">Загальні вказівки з ефективності перенесення</span><span class="sxs-lookup"><span data-stu-id="f0015-102">General migration performance guidance</span></span>

<span data-ttu-id="f0015-103">**Важливо**. Багато клієнтів SharePoint Online і OneDrive запускають у службі критично важливі для бізнесу програми, що працюють у фоновому режимі.</span><span class="sxs-lookup"><span data-stu-id="f0015-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="f0015-104">До них належать перенесення вмісту, захист від втрати даних (DLP) і рішення для резервного копіювання.</span><span class="sxs-lookup"><span data-stu-id="f0015-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="f0015-105">У цей безпрецедентний час ми працюємо над тим, щоб служби SharePoint Online і OneDrive залишалися високодоступними та надійними для користувачів, які залежать від них більше, ніж будь-коли, через віддалену роботу.</span><span class="sxs-lookup"><span data-stu-id="f0015-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="f0015-106">З цією метою ми впровадили жорсткіші обмеження кількості запитів для фонових програм (перенесення, DLP та рішення для резервного копіювання) у денний час у будні дні.</span><span class="sxs-lookup"><span data-stu-id="f0015-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="f0015-107">Слід очікувати, що пропускну здатність цих програм буде дуже сильно обмежено протягом цього часу.</span><span class="sxs-lookup"><span data-stu-id="f0015-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="f0015-108">Проте у вечірній час та по вихідних (для конкретного регіону) служба зможе обробляти значно більший обсяг запитів від фонових програм.</span><span class="sxs-lookup"><span data-stu-id="f0015-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="f0015-109">**Вказівки з ефективності перенесення**</span><span class="sxs-lookup"><span data-stu-id="f0015-109">**Migration performance guidance**</span></span>

<span data-ttu-id="f0015-110">На ефективність перенесення можуть впливати мережева інфраструктура, розмір файлу, час перенесення та обмеження.</span><span class="sxs-lookup"><span data-stu-id="f0015-110">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling.</span></span> <span data-ttu-id="f0015-111">Розуміння цього допоможе вам планувати та максимально підвищити ефективність перенесення.</span><span class="sxs-lookup"><span data-stu-id="f0015-111">Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

- [<span data-ttu-id="f0015-112">Загальні вказівки з ефективності перенесення</span><span class="sxs-lookup"><span data-stu-id="f0015-112">General migration performance guidance</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)
