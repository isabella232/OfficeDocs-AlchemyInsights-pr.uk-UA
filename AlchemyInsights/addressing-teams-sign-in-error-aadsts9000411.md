---
title: Вирішення проблеми входу в групи AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: b70f1320ea1dfa29e6fa489bd02acfcd1d92971b
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/20/2020
ms.locfileid: "44358365"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="3f3bb-102">Вирішення проблеми входу в групи AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="3f3bb-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="3f3bb-103">Під час входу до Microsoft teams може з'явитися повідомлення про помилку: **Вибачте, але у нас виникли проблеми з підписуванням вас у AADSTS9000411: запит не відформатовано належним чином. Параметр "login_hint" дублюється.**</span><span class="sxs-lookup"><span data-stu-id="3f3bb-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="3f3bb-104">Щоб вирішити цю проблему, переконайтеся, що клієнти Microsoft teams оновлюються.</span><span class="sxs-lookup"><span data-stu-id="3f3bb-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="3f3bb-105">Докладніші відомості про оновлення клієнта наведено в [оновленні Microsoft teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="3f3bb-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="3f3bb-106">Якщо ви не можете оновити свій клієнт чомусь, увійшовши в систему, клієнт буде очищати більшість кешованих даних.</span><span class="sxs-lookup"><span data-stu-id="3f3bb-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="3f3bb-107">Однак, якщо у вас ще є проблеми після виходу з системи/входу в систему, закрийте групи і будь ласка, Очистіть кеш клієнта, виконавши такі дії:</span><span class="sxs-lookup"><span data-stu-id="3f3bb-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="3f3bb-108">Закрийте Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="3f3bb-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="3f3bb-109">Перейти до:%appdate%\mice\prsі видалити всі файли.</span><span class="sxs-lookup"><span data-stu-id="3f3bb-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="3f3bb-110">Знову відкрийте Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="3f3bb-110">Reopen Microsoft Teams.</span></span>
