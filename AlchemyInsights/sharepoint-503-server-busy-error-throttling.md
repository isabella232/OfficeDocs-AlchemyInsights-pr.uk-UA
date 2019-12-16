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
ms.openlocfilehash: 5fdbb315698a58145e5437b0a7b127ce0062a76f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048637"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="51251-102">Регулювання SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="51251-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="51251-103">Користувачі можуть отримувати 503 сервер зайнятий, помилка під час спроби перейти до SharePoint або OneDrive сайтів.</span><span class="sxs-lookup"><span data-stu-id="51251-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="51251-104">Ця помилка може бути викликана дроселювання у службі SharePoint.</span><span class="sxs-lookup"><span data-stu-id="51251-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="51251-105">SharePoint Online використовує дроселювання для підтримки оптимальної продуктивності та надійності служби SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="51251-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="51251-106">Дроселювання обмежує кількість дій користувача або одночасних викликів (за сценарієм або кодом) для запобігання надмірного використання ресурсів.</span><span class="sxs-lookup"><span data-stu-id="51251-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="51251-107">Якщо ви отримаєте обмежив, 99% від часу, що це з-за користувацького коду.</span><span class="sxs-lookup"><span data-stu-id="51251-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="51251-108">Для отримання додаткових відомостей про дроселювання можна [уникнути обмеження або блокування в SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="51251-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="51251-109">Якщо ви вважаєте, що ця помилка не пов'язана з дроселювання, ви можете перевірити, чи є активне обслуговування, що відбувається на вашому клієнті, перейшовши до [центру повідомлень](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="51251-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="51251-110">Нарешті, переконайтеся, що ви відвідаєте сторінку [служби охорони здоров'я](https://portal.office.com/adminportal/home#/servicehealth) , щоб перевірити наявність будь-яких рекомендації/інцидентів, які можуть трапитися.</span><span class="sxs-lookup"><span data-stu-id="51251-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

