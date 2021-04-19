---
title: Помилка входу в Teams AADSTS9000411
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822008"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="51ff7-102">Помилка входу в Teams AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="51ff7-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="51ff7-103">Під час входу в Microsoft Teams може з'явитися повідомлення про помилку: На жаль, у нас виникли проблеми з входом **у AADSTS9000411. Запит відформатовано неправильно. Буде дубльовано login_hint параметр.**</span><span class="sxs-lookup"><span data-stu-id="51ff7-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="51ff7-104">Щоб вирішити цю проблему, переконайтеся, що ваші клієнти Microsoft Teams оновлено.</span><span class="sxs-lookup"><span data-stu-id="51ff7-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="51ff7-105">Докладні відомості про оновлення клієнта див. в [статті Оновлення Microsoft Teams.](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)</span><span class="sxs-lookup"><span data-stu-id="51ff7-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="51ff7-106">Якщо з якоїсь причини не вдається оновити клієнт, буде очищено більшість кешованих даних.</span><span class="sxs-lookup"><span data-stu-id="51ff7-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="51ff7-107">Однак якщо проблеми не зникли після входу або виходу з системи, закрийте Teams і очистіть кеш клієнта, виконавши такі дії:</span><span class="sxs-lookup"><span data-stu-id="51ff7-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="51ff7-108">Закрийте Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="51ff7-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="51ff7-109">Перейдіть до папки: %appdata%\microsoft\teams і видаліть усі файли.</span><span class="sxs-lookup"><span data-stu-id="51ff7-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="51ff7-110">Знову відкрити Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="51ff7-110">Reopen Microsoft Teams.</span></span>
