---
title: Створення групи
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816393"
---
# <a name="create-a-group"></a><span data-ttu-id="ab856-102">Створення групи</span><span class="sxs-lookup"><span data-stu-id="ab856-102">Create a group</span></span>

<span data-ttu-id="ab856-103">У цій статті описано створення груп.</span><span class="sxs-lookup"><span data-stu-id="ab856-103">This topic describes group creation.</span></span>

<span data-ttu-id="ab856-104">**Дозвіл на створення групи**</span><span class="sxs-lookup"><span data-stu-id="ab856-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="ab856-105">Переконайтеся, що ви маєте право створювати нову групу.</span><span class="sxs-lookup"><span data-stu-id="ab856-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="ab856-106">Глобальні адміністратори можуть вимкнути створення груп на порталі Azure або на панелі доступу.</span><span class="sxs-lookup"><span data-stu-id="ab856-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="ab856-107">Може знадобитися адміністратор, щоб створити нову групу для вас або надати вам відповідні дозволи.</span><span class="sxs-lookup"><span data-stu-id="ab856-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="ab856-108">**Керування дозволами на створення груп**</span><span class="sxs-lookup"><span data-stu-id="ab856-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="ab856-109">Глобальні адміністратори можуть керувати дозволами на створення груп (з міркувань безпеки) або групами Office 365, створеними на порталі Azure або панелі доступу, вибравши в розділі "Користувачі можуть створювати групи безпеки на порталах Azure" або "Користувачі можуть створювати групи Office 365 на порталах Azure" в розділі Загальні  >  **групи (параметри)**.</span><span class="sxs-lookup"><span data-stu-id="ab856-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="ab856-110">Крім того, ви можете обмежити створення груп, щоб вибрати групу користувачів, якщо у вас є ліцензія Azure Active Directory P1 Premium.</span><span class="sxs-lookup"><span data-stu-id="ab856-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="ab856-111">**Вимкнення привітання для нових учасників групи Office 365**</span><span class="sxs-lookup"><span data-stu-id="ab856-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="ab856-112">Сповіщення про привітання, надіслане користувачам, які додаються до груп Office 365, можна вимкнути, установивши в PowerShell параметр **UnifiedGroupWelcomeMessageEnabled** для False.</span><span class="sxs-lookup"><span data-stu-id="ab856-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="ab856-113">Відомості про цю настройку [див. тут.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="ab856-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

