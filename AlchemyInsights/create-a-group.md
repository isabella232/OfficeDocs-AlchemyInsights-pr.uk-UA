---
title: Створення групи
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 11/17/2020
ms.locfileid: "49089180"
---
# <a name="create-a-group"></a><span data-ttu-id="3fcc9-102">Створення групи</span><span class="sxs-lookup"><span data-stu-id="3fcc9-102">Create a group</span></span>

<span data-ttu-id="3fcc9-103">У цій статті розповідається про створення групи.</span><span class="sxs-lookup"><span data-stu-id="3fcc9-103">This topic describes group creation.</span></span>

<span data-ttu-id="3fcc9-104">**Дозвіл на створення групи**</span><span class="sxs-lookup"><span data-stu-id="3fcc9-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="3fcc9-105">Переконайтеся, що ви надали дозвіл на створення нової групи.</span><span class="sxs-lookup"><span data-stu-id="3fcc9-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="3fcc9-106">Глобальні адміністратори можуть вимкнути створення групи на веб-порталі або панелі доступу.</span><span class="sxs-lookup"><span data-stu-id="3fcc9-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="3fcc9-107">Щоб створити нову групу або надати вам відповідні дозволи, може знадобитися адміністратор.</span><span class="sxs-lookup"><span data-stu-id="3fcc9-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="3fcc9-108">**Керування дозволами на створення групи**</span><span class="sxs-lookup"><span data-stu-id="3fcc9-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="3fcc9-109">Глобальні адміністратори можуть керувати дозволами на створення групи (для причин, пов'язаних із безпекою) або групами Office 365, створеними на веб-порталі або панелі доступу, за допомогою функції "користувачі можуть створювати групи безпеки в лазуркому" або "користувачі можуть створювати групи Office 365 в розділі" блакитні портали "в **усіх групах**  >  **загальні (настройки)**.</span><span class="sxs-lookup"><span data-stu-id="3fcc9-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="3fcc9-110">Ви також можете обмежити створення групи, щоб вибрати групу користувачів, якщо у вас є ліцензія Azure Active Directory P1 Premium.</span><span class="sxs-lookup"><span data-stu-id="3fcc9-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="3fcc9-111">**Вимкнення сповіщень про привітання для нових учасників групи Office 365**</span><span class="sxs-lookup"><span data-stu-id="3fcc9-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="3fcc9-112">Сповіщення про привітання, надіслане користувачам, які додаються до груп Office 365, можна вимкнути за допомогою параметра **Unifiedgrod,** що має значення FALSE в PowerShell.</span><span class="sxs-lookup"><span data-stu-id="3fcc9-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="3fcc9-113">Дізнайтеся про [цю настройку.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="3fcc9-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

