---
title: Проблеми з ліцензування Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657297"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="0fe23-102">Проблеми з ліцензування Yammer</span><span class="sxs-lookup"><span data-stu-id="0fe23-102">Yammer licensing issues</span></span>

<span data-ttu-id="0fe23-103">Усі користувачі повинні мати ліцензію на використання служби "Yammer Enterprise Service", але за замовчуванням Yammer не вимагає, щоб користувачі мали ліцензію на доступ до служби.</span><span class="sxs-lookup"><span data-stu-id="0fe23-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="0fe23-104">Якщо адміністратор змінив параметр для блокування користувачів Microsoft 365 без ліцензій Yammer, користувачі, які не мають ліцензії Yammer Enterprise, не можуть отримати доступ до служби Yammer.</span><span class="sxs-lookup"><span data-stu-id="0fe23-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="0fe23-105">Докладні відомості наведено в статті [керування ліцензіями користувачів Yammer в Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="0fe23-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="0fe23-106">Коли ліцензії буде видалено з користувачів, плитку Yammer більше не відображається, а інші служби можуть використовувати засіб видалення ліцензій, щоб приховати функції.</span><span class="sxs-lookup"><span data-stu-id="0fe23-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="0fe23-107">В інших випадках функції все ще можуть відображатися, але для роботи з ним потрібно мати ліцензію.</span><span class="sxs-lookup"><span data-stu-id="0fe23-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="0fe23-108">**Ліцензія не оновлюється для користувача**</span><span class="sxs-lookup"><span data-stu-id="0fe23-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="0fe23-109">Час від часу користувача призначається ліцензія, але вона все ще не може отримати доступ до Yammer.</span><span class="sxs-lookup"><span data-stu-id="0fe23-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="0fe23-110">Скоріш за все, після виконання завдання з масовою ліцензією відбувається затримка.</span><span class="sxs-lookup"><span data-stu-id="0fe23-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="0fe23-111">Користувачі Yammer можуть не оновлюватись в тому ж порядку, що й ліцензії змінено в Azure AD, оскільки система працює асинхронно.</span><span class="sxs-lookup"><span data-stu-id="0fe23-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="0fe23-112">Зачекайте до 24 годин, перш ніж відкрити інцидент підтримки, щоб повідомити про проблеми з синхронізацією ліцензії.</span><span class="sxs-lookup"><span data-stu-id="0fe23-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="0fe23-113">**Масове призначення ліцензії**</span><span class="sxs-lookup"><span data-stu-id="0fe23-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="0fe23-114">Ліцензії можна призначати через центр адміністрування або сценарії PowerShell.</span><span class="sxs-lookup"><span data-stu-id="0fe23-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="0fe23-115">Докладні відомості наведено в статті [призначення ліцензій користувачам](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) і [призначення ліцензій для облікових записів користувачів із програмою Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="0fe23-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="0fe23-116">Служба підтримки Microsoft не надає допомогу зі створення сценаріїв, але доступна документація до призначення ліцензії Yammer.</span><span class="sxs-lookup"><span data-stu-id="0fe23-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="0fe23-117">Докладні відомості наведено в статті [керування ліцензіями Yammer за допомогою оболонки Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="0fe23-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>