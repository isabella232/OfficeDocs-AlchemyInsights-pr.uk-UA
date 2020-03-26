---
title: Ефективність перенесення
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
- "2700"
ms.openlocfilehash: 812444589d5a5bf766bbc6f466077d4ca829d79f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932409"
---
# <a name="sharepoint-migration-performance"></a><span data-ttu-id="61828-102">Ефективність перенесення</span><span class="sxs-lookup"><span data-stu-id="61828-102">SharePoint migration performance</span></span>

<span data-ttu-id="61828-103">**Важливо**. Багато клієнтів SharePoint Online і OneDrive запускають у службі критично важливі для бізнесу програми, що працюють у фоновому режимі.</span><span class="sxs-lookup"><span data-stu-id="61828-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="61828-104">До них належать перенесення вмісту, захист від втрати даних (DLP) і рішення для резервного копіювання.</span><span class="sxs-lookup"><span data-stu-id="61828-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="61828-105">У цей безпрецедентний час ми працюємо над тим, щоб служби SharePoint Online і OneDrive залишалися високодоступними та надійними для користувачів, які залежать від них більше, ніж будь-коли, через віддалену роботу.</span><span class="sxs-lookup"><span data-stu-id="61828-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="61828-106">З цією метою ми впровадили жорсткіші обмеження кількості запитів для фонових програм (перенесення, DLP та рішення для резервного копіювання) у денний час у будні дні.</span><span class="sxs-lookup"><span data-stu-id="61828-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="61828-107">Слід очікувати, що пропускну здатність цих програм буде дуже сильно обмежено протягом цього часу.</span><span class="sxs-lookup"><span data-stu-id="61828-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="61828-108">Проте у вечірній час та по вихідних (для конкретного регіону) служба зможе обробляти значно більший обсяг запитів від фонових програм.</span><span class="sxs-lookup"><span data-stu-id="61828-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="61828-109">**Ефективність перенесення**</span><span class="sxs-lookup"><span data-stu-id="61828-109">**Migration performance**</span></span>

<span data-ttu-id="61828-110">На ефективність перенесення можуть впливати мережева інфраструктура, розмір файлу, час перенесення та обмеження.</span><span class="sxs-lookup"><span data-stu-id="61828-110">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling.</span></span> <span data-ttu-id="61828-111">Розуміння цього допоможе вам планувати та максимально підвищити ефективність перенесення.</span><span class="sxs-lookup"><span data-stu-id="61828-111">Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

<span data-ttu-id="61828-112">Щоб дізнатися більше, перейдіть за посиланнями нижче.</span><span class="sxs-lookup"><span data-stu-id="61828-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="61828-113">SharePoint Online і швидкість перенесення у OneDrive для бізнесу</span><span class="sxs-lookup"><span data-stu-id="61828-113">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="61828-114">Уникнення обмеження або блокування в SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="61828-114">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="61828-115">Завантаження та інсталяція інструмента перенесення даних SharePoint</span><span class="sxs-lookup"><span data-stu-id="61828-115">Download and install the SharePoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)
