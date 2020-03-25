---
title: Усунення проблем із засобом міграції SharePoint проблеми та помилки
ms.author: v-miegge
author: v-miegge
manager: v-cojank
ms.date: 10/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3178"
ms.assetid: ''
ms.openlocfilehash: f9f5694b1d88bccebdc5448d5629ea5120c52511
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931139"
---
# <a name="troubleshooting-sharepoint-migration-tool-issues-and-errors"></a><span data-ttu-id="759da-102">Усунення проблем із засобом міграції SharePoint проблеми та помилки</span><span class="sxs-lookup"><span data-stu-id="759da-102">Troubleshooting SharePoint Migration Tool issues and errors</span></span>

<span data-ttu-id="759da-103">**Важливо**: багато SharePoint Online і OneDrive клієнтів, запустіть бізнес-критичних програм від служби, які працюють у фоновому режимі.</span><span class="sxs-lookup"><span data-stu-id="759da-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="759da-104">До них відносяться міграція вмісту, запобігання втрати даних (ЗВД) і рішення для резервного копіювання.</span><span class="sxs-lookup"><span data-stu-id="759da-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="759da-105">У ці безпрецедентні часи Ми вживаємо заходів, щоб гарантувати, що служби SharePoint Online та OneDrive залишаються дуже доступними та надійними для користувачів, які залежать від служби, ніж будь-коли в віддалених сценаріях роботи.</span><span class="sxs-lookup"><span data-stu-id="759da-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="759da-106">На підтримку цієї мети, ми реалізували жорсткі обмеження регулювання на фонових програм (міграція, ЗВД і резервне копіювання рішень) в будні дні вдень.</span><span class="sxs-lookup"><span data-stu-id="759da-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="759da-107">Ви повинні очікувати, що ці програми будуть досягати дуже обмежену пропускну здатність в ці часи.</span><span class="sxs-lookup"><span data-stu-id="759da-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="759da-108">Однак під час вечірніх та вихідних годин для регіону служба буде готова обробляти значно більший обсяг запитів від фонових програм.</span><span class="sxs-lookup"><span data-stu-id="759da-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="759da-109">**Поширені проблеми та помилки**</span><span class="sxs-lookup"><span data-stu-id="759da-109">**Common issues and errors**</span></span>

<span data-ttu-id="759da-110">Під час використання засобу міграції SharePoint (SPMT) можуть виникати деякі поширені проблеми та помилки.</span><span class="sxs-lookup"><span data-stu-id="759da-110">You may encounter some common issues and errors when using the SharePoint Migration Tool (SPMT).</span></span> <span data-ttu-id="759da-111">Будь ласка, посилання на посилання нижче для отримання додаткової інформації.</span><span class="sxs-lookup"><span data-stu-id="759da-111">Please reference the links below for more information.</span></span>

* [<span data-ttu-id="759da-112">Усунення несправностей, поширених проблем і помилок SPMT</span><span class="sxs-lookup"><span data-stu-id="759da-112">Troubleshooting common SPMT issues and errors</span></span>](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
* [<span data-ttu-id="759da-113">Усунення проблем із інсталяцією SPMT</span><span class="sxs-lookup"><span data-stu-id="759da-113">Troubleshooting SPMT install issues</span></span>](https://docs.microsoft.com/sharepointmigration/spmt-install-issues)