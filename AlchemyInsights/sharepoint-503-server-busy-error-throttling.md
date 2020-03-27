---
title: Регулювання SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 2aca55ac2fefbb2035140a759a77730dc905a4e9
ms.sourcegitcommit: 926e4ab6aa64ddc7a244de633421eb2b817541f2
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/26/2020
ms.locfileid: "42958756"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="63c7c-102">Регулювання SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="63c7c-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="63c7c-103">**Важливо**: у ці безпрецедентні часи Ми вживаємо заходів, щоб гарантувати, що служби SharePoint Online та OneDrive залишаються доступними – будь ласка, відвідайте [тимчасові функції SharePoint Online](https://aka.ms/ODSPAdjustments) для отримання додаткових відомостей.</span><span class="sxs-lookup"><span data-stu-id="63c7c-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="63c7c-104">**503 сервер зайнятий, помилка**</span><span class="sxs-lookup"><span data-stu-id="63c7c-104">**503 server is busy error**</span></span>

<span data-ttu-id="63c7c-105">Користувачі можуть отримувати 503 сервер зайнятий, помилка під час спроби перейти до SharePoint або OneDrive сайтів.</span><span class="sxs-lookup"><span data-stu-id="63c7c-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="63c7c-106">Ця помилка може бути викликана дроселювання у службі SharePoint.</span><span class="sxs-lookup"><span data-stu-id="63c7c-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="63c7c-107">SharePoint Online використовує дроселювання для підтримки оптимальної продуктивності та надійності служби SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="63c7c-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="63c7c-108">Дроселювання обмежує кількість дій користувача або одночасних викликів (за сценарієм або кодом) для запобігання надмірного використання ресурсів.</span><span class="sxs-lookup"><span data-stu-id="63c7c-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="63c7c-109">Для отримання додаткових відомостей про дроселювання можна [уникнути обмеження або блокування в SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="63c7c-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="63c7c-110">Якщо ви вважаєте, що ця помилка не пов'язана з дроселювання, ви можете перевірити, чи є активне обслуговування, що відбувається на вашому клієнті, перейшовши до [центру повідомлень](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="63c7c-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="63c7c-111">Нарешті, переконайтеся, що ви відвідаєте сторінку [служби охорони здоров'я](https://portal.office.com/adminportal/home#/servicehealth) , щоб перевірити наявність будь-яких рекомендації/інцидентів, які можуть трапитися.</span><span class="sxs-lookup"><span data-stu-id="63c7c-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

