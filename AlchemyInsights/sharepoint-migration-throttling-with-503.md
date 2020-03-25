---
title: Перенесення міграції SharePoint з помилками 503
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931679"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a><span data-ttu-id="20fa1-102">Перенесення міграції SharePoint з помилками 503</span><span class="sxs-lookup"><span data-stu-id="20fa1-102">SharePoint migration throttling with 503 errors</span></span>

<span data-ttu-id="20fa1-103">**Важливо**: багато SharePoint Online і OneDrive клієнтів, запустіть бізнес-критичних програм від служби, які працюють у фоновому режимі.</span><span class="sxs-lookup"><span data-stu-id="20fa1-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="20fa1-104">До них відносяться міграція вмісту, запобігання втрати даних (ЗВД) і рішення для резервного копіювання.</span><span class="sxs-lookup"><span data-stu-id="20fa1-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="20fa1-105">У ці безпрецедентні часи Ми вживаємо заходів, щоб гарантувати, що служби SharePoint Online та OneDrive залишаються дуже доступними та надійними для користувачів, які залежать від служби, ніж будь-коли в віддалених сценаріях роботи.</span><span class="sxs-lookup"><span data-stu-id="20fa1-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="20fa1-106">На підтримку цієї мети, ми реалізували жорсткі обмеження регулювання на фонових програм (міграція, ЗВД і резервне копіювання рішень) в будні дні вдень.</span><span class="sxs-lookup"><span data-stu-id="20fa1-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="20fa1-107">Ви повинні очікувати, що ці програми будуть досягати дуже обмежену пропускну здатність в ці часи.</span><span class="sxs-lookup"><span data-stu-id="20fa1-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="20fa1-108">Однак під час вечірніх та вихідних годин для регіону служба буде готова обробляти значно більший обсяг запитів від фонових програм.</span><span class="sxs-lookup"><span data-stu-id="20fa1-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="20fa1-109">**503 помилки під час переходу до SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="20fa1-109">**503 errors when migrating to SharePoint Online**</span></span>

<span data-ttu-id="20fa1-110">Схоже, ви переходите до SharePoint Online та отримання 503 помилок.</span><span class="sxs-lookup"><span data-stu-id="20fa1-110">It appears you are migrating to SharePoint Online and receiving 503 errors.</span></span> <span data-ttu-id="20fa1-111">Будь ласка, виконайте наведені нижче дії, щоб ми могли допомогти вам якомога швидше.</span><span class="sxs-lookup"><span data-stu-id="20fa1-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="20fa1-112">Натисніть кнопку, **зверніться до служби підтримки**та **новий запит на обслуговування**.</span><span class="sxs-lookup"><span data-stu-id="20fa1-112">Click **Contact Support**, and then **New Service Request**.</span></span>
2. <span data-ttu-id="20fa1-113">Заголовок і Опис введіть **дроселювання міграції SharePoint за допомогою 503**.</span><span class="sxs-lookup"><span data-stu-id="20fa1-113">For the title and description, type **SharePoint Migration Throttling with 503**.</span></span>
3. <span data-ttu-id="20fa1-114">Після того, як квиток був представлений, будь ласка, поновіть його з наступною інформацією:</span><span class="sxs-lookup"><span data-stu-id="20fa1-114">Once the ticket has been submitted, please update it with the following information:</span></span>
    - <span data-ttu-id="20fa1-115">Скільки залишилося міграції (наприклад, скільки TBs?).</span><span class="sxs-lookup"><span data-stu-id="20fa1-115">How much left of migration (for example, how many TBs?).</span></span>
    - <span data-ttu-id="20fa1-116">Дата початку та завершення міграції.</span><span class="sxs-lookup"><span data-stu-id="20fa1-116">Migration start and end date.</span></span>
    - <span data-ttu-id="20fa1-117">Опишіть, де ви переміщуєте ваш вміст, наприклад, сервер SharePoint, коробка, GDrive, спільний доступ до файлів тощо.</span><span class="sxs-lookup"><span data-stu-id="20fa1-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>
    - <span data-ttu-id="20fa1-118">Оцініть кількість похибок дроселювання (наприклад, x дроселя на годину?) і коли відбувається дроселювання.</span><span class="sxs-lookup"><span data-stu-id="20fa1-118">Estimate the number of throttling errors (for example, x throttle per hour?) and when did the throttling happen.</span></span>
    - <span data-ttu-id="20fa1-119">Який інструмент міграції використовується (наприклад, SPMT або ShareGate).</span><span class="sxs-lookup"><span data-stu-id="20fa1-119">Which migration tool you are using (for example, SPMT or ShareGate).</span></span>


