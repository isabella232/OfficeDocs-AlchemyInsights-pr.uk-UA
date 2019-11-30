---
title: Розташування даних
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: ec8fb91dfe77cb251579ce23eb0579b114b101d9
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627867"
---
# <a name="data-location"></a><span data-ttu-id="8ed4a-102">Розташування даних</span><span class="sxs-lookup"><span data-stu-id="8ed4a-102">Data location</span></span>

<span data-ttu-id="8ed4a-103">Ви можете переглянути розташування вашого клієнта Office 365 в центрі адміністрування або шляхом підключення до Exchange Online через PowerShell.</span><span class="sxs-lookup"><span data-stu-id="8ed4a-103">You can view the location of your Office 365 tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="8ed4a-104">**Центр адміністрування:**</span><span class="sxs-lookup"><span data-stu-id="8ed4a-104">**Admin center:**</span></span>
1. <span data-ttu-id="8ed4a-105">Увійдіть в [Центр адміністрування](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="8ed4a-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="8ed4a-106">Виберіть \*\*\*\* > **профіль організації**настройки.</span><span class="sxs-lookup"><span data-stu-id="8ed4a-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="8ed4a-107">У розділі **розташування даних**виберіть **переглянути деталі**.</span><span class="sxs-lookup"><span data-stu-id="8ed4a-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="8ed4a-108">**Powershell:**</span><span class="sxs-lookup"><span data-stu-id="8ed4a-108">**PowerShell:**</span></span>
1. <span data-ttu-id="8ed4a-109">Підключення до Exchange Online за допомогою оболонки Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="8ed4a-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="8ed4a-110">Виконати командлет [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) для відображення списку властивостей вашого клієнта.</span><span class="sxs-lookup"><span data-stu-id="8ed4a-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant’s properties.</span></span> 
3. <span data-ttu-id="8ed4a-111">Подивіться на власність Організаціїid.</span><span class="sxs-lookup"><span data-stu-id="8ed4a-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="8ed4a-112">Якщо у вас є дані розташування для EXO і спо, ви можете визначити розташування даних для інших послуг, які ви можете використовувати, [де ваші дані знаходяться](https://products.office.com/where-is-your-data-located).</span><span class="sxs-lookup"><span data-stu-id="8ed4a-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>