---
title: Дозволяйте та вимикайте IP-відео в Teams
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
- "9002537"
- "5617"
ms.openlocfilehash: 059d7a1ad619e25f14bc6f561693b6fe24355132
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826364"
---
# <a name="teams-allow-or-disable-ip-video"></a><span data-ttu-id="fcf84-102">Дозволяйте та вимикайте IP-відео в Teams</span><span class="sxs-lookup"><span data-stu-id="fcf84-102">Teams allow or disable IP video</span></span>

<span data-ttu-id="fcf84-103">**Змінення або створення політики наради**</span><span class="sxs-lookup"><span data-stu-id="fcf84-103">**Change or create a meeting policy**</span></span>

<span data-ttu-id="fcf84-104">Щоб змінити або створити політику наради, перейдіть у Центр адміністрування **Microsoft Teams > Наради > політику нарад.**</span><span class="sxs-lookup"><span data-stu-id="fcf84-104">To change or create a meeting policy, go to the **Microsoft Teams admin center > Meetings > Meeting policies**.</span></span> <span data-ttu-id="fcf84-105">Виберіть політику зі списку або натисніть кнопку **Додати**.</span><span class="sxs-lookup"><span data-stu-id="fcf84-105">Select a policy from the list or click **Add**.</span></span> <span data-ttu-id="fcf84-106">Якщо ви створюєте нову політику, додайте ім'я та опис.</span><span class="sxs-lookup"><span data-stu-id="fcf84-106">If you're creating a new policy, add a name and description.</span></span> <span data-ttu-id="fcf84-107">Ім'я не може містити спеціальні символи або більше 64 символів.</span><span class="sxs-lookup"><span data-stu-id="fcf84-107">The name can't contain special characters or be longer than 64 characters.</span></span> <span data-ttu-id="fcf84-108">Виберіть параметри та натисніть кнопку **Зберегти**.</span><span class="sxs-lookup"><span data-stu-id="fcf84-108">Choose your settings, and then click **Save**.</span></span>

<span data-ttu-id="fcf84-109">Скажімо, у вас багато користувачів, і вам потрібно обмежити смугу пропускання, потрібну для їхньої наради.</span><span class="sxs-lookup"><span data-stu-id="fcf84-109">For example, say you have many users and you want to limit the amount of bandwidth that their meeting would require.</span></span> <span data-ttu-id="fcf84-110">Ви можете створити нову настроювану політику під назвою "Смуга пропускання з обмеженою шириною" та вимкнути наведені нижче параметри.</span><span class="sxs-lookup"><span data-stu-id="fcf84-110">You would create a new custom policy named "Limited bandwidth" and disable the following settings:</span></span>

<span data-ttu-id="fcf84-111">У розділі **Звук і відео**:</span><span class="sxs-lookup"><span data-stu-id="fcf84-111">Under **Audio & video**:</span></span>

- <span data-ttu-id="fcf84-112">Вимкніть "Дозволити хмарне записування".</span><span class="sxs-lookup"><span data-stu-id="fcf84-112">Turn off Allow cloud recording.</span></span>
- <span data-ttu-id="fcf84-113">Вимкніть "Дозволити IP-відеозв’язок".</span><span class="sxs-lookup"><span data-stu-id="fcf84-113">Turn off Allow IP video.</span></span>

<span data-ttu-id="fcf84-114">Після цього призначте політику користувачам.</span><span class="sxs-lookup"><span data-stu-id="fcf84-114">Then assign the policy to the users.</span></span>

<span data-ttu-id="fcf84-115">**Призначення політики наради користувачам**</span><span class="sxs-lookup"><span data-stu-id="fcf84-115">**Assign a meeting policy to users**</span></span>

1. <span data-ttu-id="fcf84-116">В області переходів ліворуч у Центрі адміністрування Microsoft Teams виберіть **Користувачі**, а потім клацніть потрібного користувача.</span><span class="sxs-lookup"><span data-stu-id="fcf84-116">In the left navigation of the Microsoft Teams admin center, go to **Users**, and then click the user.</span></span>
2. <span data-ttu-id="fcf84-117">Виберіть користувача, клацнувши ліворуч від його імені, і натисніть кнопку **Редагувати параметри**.</span><span class="sxs-lookup"><span data-stu-id="fcf84-117">Select the user by clicking to the left of the user name, and then click **Edit settings**.</span></span>
3. <span data-ttu-id="fcf84-118">У **розділі Політика наради** виберіть політику, яку потрібно призначити, а потім натисніть кнопку **Застосувати**.</span><span class="sxs-lookup"><span data-stu-id="fcf84-118">Under **Meeting policy**, select the policy you want to assign and then click **Apply**.</span></span>

<span data-ttu-id="fcf84-119">Докладні відомості див. в [розділі Керування політиками нарад у Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="fcf84-119">For more information, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>
