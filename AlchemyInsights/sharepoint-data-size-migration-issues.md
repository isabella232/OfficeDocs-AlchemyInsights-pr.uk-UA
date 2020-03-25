---
title: Проблеми під час міграції даних до SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "1885"
ms.openlocfilehash: b53a98480bab48497274c7358f7e606caa477f5a
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931715"
---
# <a name="issues-while-migrating-data-to-sharepoint-online"></a><span data-ttu-id="7cb71-102">Проблеми під час міграції даних до SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="7cb71-102">Issues while migrating data to SharePoint Online</span></span>

<span data-ttu-id="7cb71-103">**Важливо**: багато SharePoint Online і OneDrive клієнтів, запустіть бізнес-критичних програм від служби, які працюють у фоновому режимі.</span><span class="sxs-lookup"><span data-stu-id="7cb71-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="7cb71-104">До них відносяться міграція вмісту, запобігання втрати даних (ЗВД) і рішення для резервного копіювання.</span><span class="sxs-lookup"><span data-stu-id="7cb71-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="7cb71-105">У ці безпрецедентні часи Ми вживаємо заходів, щоб гарантувати, що служби SharePoint Online та OneDrive залишаються дуже доступними та надійними для користувачів, які залежать від служби, ніж будь-коли в віддалених сценаріях роботи.</span><span class="sxs-lookup"><span data-stu-id="7cb71-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="7cb71-106">На підтримку цієї мети, ми реалізували жорсткі обмеження регулювання на фонових програм (міграція, ЗВД і резервне копіювання рішень) в будні дні вдень.</span><span class="sxs-lookup"><span data-stu-id="7cb71-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="7cb71-107">Ви повинні очікувати, що ці програми будуть досягати дуже обмежену пропускну здатність в ці часи.</span><span class="sxs-lookup"><span data-stu-id="7cb71-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="7cb71-108">Однак під час вечірніх та вихідних годин для регіону служба буде готова обробляти значно більший обсяг запитів від фонових програм.</span><span class="sxs-lookup"><span data-stu-id="7cb71-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="7cb71-109">**Міграція понад 100 ТБ даних**</span><span class="sxs-lookup"><span data-stu-id="7cb71-109">**Migrating over 100TB of data**</span></span>

<span data-ttu-id="7cb71-110">Схоже, ви переходите на 100 ТБ даних до SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="7cb71-110">It appears you are migrating over 100TB of data to SharePoint Online.</span></span> <span data-ttu-id="7cb71-111">Будь ласка, виконайте наведені нижче дії, щоб ми могли допомогти вам якомога швидше.</span><span class="sxs-lookup"><span data-stu-id="7cb71-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="7cb71-112">Виберіть **новий запит на обслуговування**, а потім **новий запит на обслуговування**.</span><span class="sxs-lookup"><span data-stu-id="7cb71-112">Select **New Service Request**, and then **New Service Request**.</span></span> 
2. <span data-ttu-id="7cb71-113">Залиште заголовок і опис як **SharePoint міграція більше 100 ТБ**.</span><span class="sxs-lookup"><span data-stu-id="7cb71-113">Leave the title and description as **SharePoint migration over 100TB**.</span></span>
3. <span data-ttu-id="7cb71-114">Після того, як квиток був представлений, будь ласка, поновіть його з наступною інформацією:</span><span class="sxs-lookup"><span data-stu-id="7cb71-114">Once the ticket has been submitted, please update it with the following information:</span></span> 

    - <span data-ttu-id="7cb71-115">Передбачуваний розмір вашої міграції.</span><span class="sxs-lookup"><span data-stu-id="7cb71-115">Estimated size of your migration.</span></span>
    - <span data-ttu-id="7cb71-116">Оцінка, коли ви хотіли б почати і завершити міграцію.</span><span class="sxs-lookup"><span data-stu-id="7cb71-116">An estimate of when you would like to start and complete your migration.</span></span>
    - <span data-ttu-id="7cb71-117">Опишіть, де ви переміщуєте ваш вміст, наприклад, сервер SharePoint, коробка, GDrive, спільний доступ до файлів тощо.</span><span class="sxs-lookup"><span data-stu-id="7cb71-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>


  

