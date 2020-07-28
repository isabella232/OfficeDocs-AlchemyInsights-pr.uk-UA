---
title: Як видалити окремий канал teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439910"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="e87cb-102">Як видалити окремий канал teams</span><span class="sxs-lookup"><span data-stu-id="e87cb-102">Delete a Teams private channel</span></span>

<span data-ttu-id="e87cb-103">Корпорація Майкрософт відомо про проблему видалення групи приватних каналу, якщо у вас є політики збереження SharePoint, які ввімкнуто на основний сайт SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e87cb-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="e87cb-104">Корпорація Майкрософт працює над виправленням.</span><span class="sxs-lookup"><span data-stu-id="e87cb-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="e87cb-105">У той же час, ви можете використовувати наступні способи, щоб видалити приватний канал.</span><span class="sxs-lookup"><span data-stu-id="e87cb-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="e87cb-106">**Виключіть колекцію команд/сайтів із політики збереження SharePoint.**</span><span class="sxs-lookup"><span data-stu-id="e87cb-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="e87cb-107">Перейдіть на портал адміністрування Office 365 і виберіть **Показати все** в лівій навігаційній панелі.</span><span class="sxs-lookup"><span data-stu-id="e87cb-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="e87cb-108">У **центрах адміністрування**перейдіть до політики **безпеки, & дотримання**правил  >  **запобігання втрати даних**  >  **Policy**.</span><span class="sxs-lookup"><span data-stu-id="e87cb-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="e87cb-109">Визначте будь-яку політику, яка застосовується до сайтів SharePoint, і змініть політику, тому сайт SharePoint для команди, яка містить приватний канал, не входить до політики збереження.</span><span class="sxs-lookup"><span data-stu-id="e87cb-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="e87cb-110">Збережіть політику.</span><span class="sxs-lookup"><span data-stu-id="e87cb-110">Save the policy.</span></span>
    <span data-ttu-id="e87cb-111">Щоб параметри політики набрали сили, може тривати до 24 годин.</span><span class="sxs-lookup"><span data-stu-id="e87cb-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="e87cb-112">Після виключення сайту ви можете видалити приватний канал.</span><span class="sxs-lookup"><span data-stu-id="e87cb-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="e87cb-113">Ви ***можете*** видалити приватний канал за допомогою Microsoft teams на пристрої Android.</span><span class="sxs-lookup"><span data-stu-id="e87cb-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="e87cb-114">Для пов'язаних із SharePoint відомостей див. [не вдалося видалити елементи SharePoint Online або OneDrive, для бізнесу](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span><span class="sxs-lookup"><span data-stu-id="e87cb-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>