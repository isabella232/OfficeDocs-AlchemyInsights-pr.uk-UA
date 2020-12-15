---
title: Рядок агента користувача Microsoft EDGE (робочий стіл)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003862"
- "6914"
ms.openlocfilehash: b4106dde1e09e0ce07b4b9adc2b2984cc5609c3b
ms.sourcegitcommit: 3c6e777d6679a24108171e9aa3f9379a8d44e001
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679329"
---
# <a name="microsoft-edge-user-agent-string-desktop"></a><span data-ttu-id="9e333-102">Рядок агента користувача Microsoft EDGE (робочий стіл)</span><span class="sxs-lookup"><span data-stu-id="9e333-102">Microsoft Edge user agent string (Desktop)</span></span>

<span data-ttu-id="9e333-103">Рядки агента користувача (UA) можна використовувати, щоб визначити, яка версія певного браузера використовується для певної операційної системи.</span><span class="sxs-lookup"><span data-stu-id="9e333-103">User agent (UA) strings can be used to detect what version of a specific browser is being used on a certain operating system.</span></span> <span data-ttu-id="9e333-104">Як і в інших браузерах, Microsoft EDGE включає цю інформацію в заголовку "Агент користувача" HTTP, коли він вносить запит на сайт.</span><span class="sxs-lookup"><span data-stu-id="9e333-104">Like other browsers, Microsoft Edge includes this information in the "User-Agent" HTTP header whenever it makes a request to a site.</span></span> <span data-ttu-id="9e333-105">Відомості про версію браузера також можна отримати за допомогою JavaScript, відповідний запит на значення "Навігатор. userAgent".</span><span class="sxs-lookup"><span data-stu-id="9e333-105">The browser-version information can also be accessed via JavaScript by querying the value of "navigator.userAgent".</span></span>

<span data-ttu-id="9e333-106">Ми радимо, що веб-розробники використовують функцію виявлення функцій, коли це можливо, щоб покращити придатність коду, зменшити крихкість коду та усунути небезпеку поломки коду в разі подальшого оновлення рядка UA.</span><span class="sxs-lookup"><span data-stu-id="9e333-106">We recommend that web developers make use of feature detection whenever possible to improve code maintainability, reduce code fragility, and eliminate the risk of code breakage in the event of future UA string updates.</span></span>

<span data-ttu-id="9e333-107">Щоб отримати докладніші відомості, ознайомтеся з [рядком агента користувача Microsoft EDGE (для настільних комп'ютерів)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span><span class="sxs-lookup"><span data-stu-id="9e333-107">For more information, see [Microsoft Edge User Agent String (Desktop)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span></span>