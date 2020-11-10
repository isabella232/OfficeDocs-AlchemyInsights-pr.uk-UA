---
title: Використання Гіфіз в розмовах команд
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982573"
---
# <a name="using-giphys-in-teams-conversations"></a><span data-ttu-id="a763d-102">Використання Гіфіз в розмовах команд</span><span class="sxs-lookup"><span data-stu-id="a763d-102">Using Giphys in Teams Conversations</span></span>

<span data-ttu-id="a763d-103">Підтримка giphys у чаті команд активовано за замовчуванням.</span><span class="sxs-lookup"><span data-stu-id="a763d-103">Giphys access in Teams chat is enabled by default.</span></span> <span data-ttu-id="a763d-104">Адміністратор може визначати, чи доступні для користувачів Giphys, [настроївши політику обміну повідомленнями](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) та **гарантуючи, що** в них **використовується функція giphys** .</span><span class="sxs-lookup"><span data-stu-id="a763d-104">As an administrator, you can control if Giphys are available to users by [setting a messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) and ensuring that **Use Giphys in conversations** is **On**.</span></span>

<span data-ttu-id="a763d-105">Якщо GIF-файли не працюють належним чином в розмовах зі командами, перевірте:</span><span class="sxs-lookup"><span data-stu-id="a763d-105">If GIFs are not working as expected in Teams conversations, verify:</span></span>

<span data-ttu-id="a763d-106">[Політика обміну повідомленнями](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) має дозволити giphys.</span><span class="sxs-lookup"><span data-stu-id="a763d-106">The [messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) needs to allow Giphys.</span></span> <span data-ttu-id="a763d-107">Щоб перевірити за допомогою командлетів PowerShell, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="a763d-107">To verify by using PowerShell cmdlets:</span></span>

- <span data-ttu-id="a763d-108">Переконайтеся, що ви можете [керувати командами за допомогою PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="a763d-108">Verify that you can [Manage Teams with PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span></span>
- <span data-ttu-id="a763d-109">Запустіть команду "Завантажити", щоб [отримати доступ](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) до цієї програми, щоб визначити, що **AllowGiphy** має значення **True**.</span><span class="sxs-lookup"><span data-stu-id="a763d-109">Run the PowerShell command [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) and verify that **AllowGiphy** is set to **TRUE**.</span></span>
- <span data-ttu-id="a763d-110">Якщо **AllowGiphy** має значення **false** , виконайте наведені нижче набір команд PowerShell [– значення політики глобального – AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="a763d-110">If **AllowGiphy** is set to **FALSE** , run the following PowerShell command [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span></span>

<span data-ttu-id="a763d-111">Щоб дозволити доступ до URL-адреси Giphy, потрібно ввімкнути [додатковий підключений досвід](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) .</span><span class="sxs-lookup"><span data-stu-id="a763d-111">[Optional Connected Experiences](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) need to be enabled to allow access to the Giphy URL.</span></span>

> [!NOTE]
> <span data-ttu-id="a763d-112">Якщо у вас є кілька політик обміну повідомленнями групи, настроєні для вашого клієнта, можна визначити ідентичність політики, призначеної для певного користувача за допомогою команди PowerShell [Get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Виберіть команду TeamsMessagingPolicy.</span><span class="sxs-lookup"><span data-stu-id="a763d-112">If you have multiple Teams Messaging policies configured for your tenant, you can determine the identity of the policy assigned to the impacted user with the PowerShell command [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Select TeamsMessagingPolicy.</span></span>
