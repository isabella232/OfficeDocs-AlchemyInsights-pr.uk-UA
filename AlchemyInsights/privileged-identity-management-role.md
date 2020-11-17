---
title: Привілейований роль керування посвідченнями
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
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 11/17/2020
ms.locfileid: "49089147"
---
# <a name="privileged-identity-managementpim-role"></a><span data-ttu-id="657f4-102">Роль в організації привілейованого посвідчення (PIM)</span><span class="sxs-lookup"><span data-stu-id="657f4-102">Privileged Identity Management(PIM) role</span></span>

<span data-ttu-id="657f4-103">**Дозволи не надаються після активації ролі**</span><span class="sxs-lookup"><span data-stu-id="657f4-103">**Permissions are not granted after activating a role**</span></span>

<span data-ttu-id="657f4-104">Коли ви активуєте роль у службі керування посвідченнями в лазурі "Лазурний" (PIM), активація може не миттєво поширюватися на всі портали, які вимагають привілейованої ролі.</span><span class="sxs-lookup"><span data-stu-id="657f4-104">When you activate a role in Azure AD Privileged Identity Management (PIM), the activation may not instantly propagate to all portals that require the privileged role.</span></span> <span data-ttu-id="657f4-105">Інколи, навіть якщо зміни розповсюджено, веб-кешування на порталі може призвести до того, що зміни не набрали чинності відразу.</span><span class="sxs-lookup"><span data-stu-id="657f4-105">Sometimes, even if the change is propagated, web caching in a portal may result in the change not taking effect immediately.</span></span>

<span data-ttu-id="657f4-106">Якщо активацію буде відкладено, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="657f4-106">If your activation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="657f4-107">Вийдіть із порталу "Лазурний", а потім знову ввійдіть у службу.</span><span class="sxs-lookup"><span data-stu-id="657f4-107">Sign out of the Azure portal and then sign back in.</span></span> <span data-ttu-id="657f4-108">Коли ви активуєте роль Лазур або роль блакитного ресурсу, ви побачите етапи активації.</span><span class="sxs-lookup"><span data-stu-id="657f4-108">When you activate an Azure AD role or an Azure resource role, you will see the stages of your activation.</span></span> <span data-ttu-id="657f4-109">Коли всі етапи будуть завершені, ви побачите посилання "вийти".</span><span class="sxs-lookup"><span data-stu-id="657f4-109">Once all the stages are complete, you will see a 'Sign out' link.</span></span> <span data-ttu-id="657f4-110">Ви можете скористатися цим посиланням, щоб вийти. Це вирішить більшість випадків, коли затримка активації буде вирішена.</span><span class="sxs-lookup"><span data-stu-id="657f4-110">You can use this link to sign out. This will solve most cases for activation delay.</span></span>
2. <span data-ttu-id="657f4-111">У PIM переконайтеся, що ви зареєстровані як учасник ролі.</span><span class="sxs-lookup"><span data-stu-id="657f4-111">In PIM, verify that you are listed as the member of the role.</span></span>
3. <span data-ttu-id="657f4-112">Якщо ви активуєте роль адміністратора Exchange, переконайтеся, що ви вийшли з редагування, і знову ввійдіть.</span><span class="sxs-lookup"><span data-stu-id="657f4-112">If you are activating the Exchange Administrator role, make sure you sign out and sign back in.</span></span> <span data-ttu-id="657f4-113">Якщо проблему не вирішено, відкрийте квиток служби підтримки та виконайте цю проблему.</span><span class="sxs-lookup"><span data-stu-id="657f4-113">If the problem persists, open a support ticket and raise this as an issue.</span></span> <span data-ttu-id="657f4-114">Якщо ви використовуєте роль адміністратора Exchange, щоб отримати доступ до центру безпеки та відповідності, ознайомтеся з наступним кроком.</span><span class="sxs-lookup"><span data-stu-id="657f4-114">If you are using your Exchange Administrator role to access the Security and Compliance Center, see the next step.</span></span>
4. <span data-ttu-id="657f4-115">Якщо ви активуєте роль, щоб отримати доступ до центру безпеки та відповідності, або якщо ви активуєте роль адміністратора SharePoint, ви отримаєте кілька хвилин на кілька годин.</span><span class="sxs-lookup"><span data-stu-id="657f4-115">If you are activating a role to access the Security and Compliance Center or if you are activating the SharePoint Administrator role, you will experience some activation delay from a few minutes up to a few hours.</span></span> <span data-ttu-id="657f4-116">Це відома проблема, і ми активно працюємо над цими командами, щоб вирішити цю проблему якомога швидше.</span><span class="sxs-lookup"><span data-stu-id="657f4-116">This is a known issue and we are actively working with these teams to resolve this issue as soon as possible.</span></span>

<span data-ttu-id="657f4-117">Докладні відомості:</span><span class="sxs-lookup"><span data-stu-id="657f4-117">For more information, see:</span></span>

- [<span data-ttu-id="657f4-118">Активація моїх ролей Лазур у PIM</span><span class="sxs-lookup"><span data-stu-id="657f4-118">Activate my Azure AD roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [<span data-ttu-id="657f4-119">Активація моїх Лазуроролей ресурсів у PIM</span><span class="sxs-lookup"><span data-stu-id="657f4-119">Activate my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

<span data-ttu-id="657f4-120">**Дозволи не видаляються після вимкнення ролі або завершення активації ролі**</span><span class="sxs-lookup"><span data-stu-id="657f4-120">**Permissions are not removed after deactivating a role or the role activation expires**</span></span>

<span data-ttu-id="657f4-121">Під час вимкнення ролі в службі керування посвідченнями в Azure AD, або коли термін активації терміну дії завершується, можливо, буде затримка, де ви будете мати доступ.</span><span class="sxs-lookup"><span data-stu-id="657f4-121">When you deactivate a role in Azure AD Privileged Identity Management or when a role activation period expires, there might be a delay where you continue to have access.</span></span>

<span data-ttu-id="657f4-122">Якщо Деактивацію затримано, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="657f4-122">If your deactivation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="657f4-123">Якщо ви відключаєте роль адміністратора Exchange або період активації ролей завершується, і ви помітите значну затримку перед видаленням дозволів, відкрийте квиток служби підтримки та повідомте інженера з підтримки, щоб допомогти вам у роботі з цією проблемою отримати квиток за допомогою команди "керування доступом" (PAM) в Office.</span><span class="sxs-lookup"><span data-stu-id="657f4-123">If you are deactivating the Exchange Administrator role or the role activation period expires, and you notice a significant delay before the permissions are removed, open a support ticket and tell your support engineer to help you file a ticket with the Privileged Access Management (PAM) team inside Office about this issue.</span></span>
2. <span data-ttu-id="657f4-124">Якщо термін активації завершився, але сеанс браузера відкрито, закрийте браузер.</span><span class="sxs-lookup"><span data-stu-id="657f4-124">If the activation period has expired, but you still have the browser session open, close your browser.</span></span> <span data-ttu-id="657f4-125">Ви можете продовжувати використовувати роль, доки не закриваєте цей сеанс.</span><span class="sxs-lookup"><span data-stu-id="657f4-125">You can continue to use the role until you close that session.</span></span> <span data-ttu-id="657f4-126">Це відома проблема, і ми шукаємо потенційні виправлення, щоб активно відкликати кожну сесію після закінчення терміну дії активації.</span><span class="sxs-lookup"><span data-stu-id="657f4-126">This is a known issue and we are looking at a potential fix to actively revoke each session once activation has expired.</span></span>

<span data-ttu-id="657f4-127">Якщо ваша затримка відрізняється від цих двох сценаріїв, відкрийте квиток підтримки.</span><span class="sxs-lookup"><span data-stu-id="657f4-127">If your delay is different than these two scenarios, please open a support ticket.</span></span>
