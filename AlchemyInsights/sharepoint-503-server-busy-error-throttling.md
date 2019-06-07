---
title: Онлайн дроселювання SharePoint
ms.author: kirks
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: b157ce22962ac1616d6e9b3a5475edaec7fed9f7
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/07/2019
ms.locfileid: "34761279"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="ec116-102">Онлайн дроселювання SharePoint</span><span class="sxs-lookup"><span data-stu-id="ec116-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="ec116-103">Користувачі можуть отримувати на 503 сервер є зайнятий помилка під час спроби перейти до сайтів SharePoint або OneDrive.</span><span class="sxs-lookup"><span data-stu-id="ec116-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="ec116-104">Ця помилка може бути викликана шляхом регулювання в рамках служби SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ec116-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="ec116-105">SharePoint Online використовує дроселювання підтримувати оптимальну продуктивність і надійність служби SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="ec116-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="ec116-106">Дроселювання межі кількість дій користувача одночасних заклики (сценарій або код) для запобігання надмірним використанням ресурсів.</span><span class="sxs-lookup"><span data-stu-id="ec116-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="ec116-107">Якщо ви отримуєте задушив, 99% часу саме через власний код.</span><span class="sxs-lookup"><span data-stu-id="ec116-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="ec116-108">Більш докладну інформацію про дроселювання див, [уникати отримання задушив або заблоковані в SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="ec116-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="ec116-109">Якщо ви вважаєте, ця помилка не має відношення до регулювання, ви можете перевірити, якщо немає активних технічне обслуговування, що відбуваються на ваш орендар, перейти на [повідомлення центру](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="ec116-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="ec116-110">Нарешті, переконайтеся, що ви відвідуєте [Служби охорони здоров'я](https://portal.office.com/adminportal/home#/servicehealth) сторінку, щоб перевірити наявність рекомендації/інцидентів, які можуть бути що відбуваються.</span><span class="sxs-lookup"><span data-stu-id="ec116-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

