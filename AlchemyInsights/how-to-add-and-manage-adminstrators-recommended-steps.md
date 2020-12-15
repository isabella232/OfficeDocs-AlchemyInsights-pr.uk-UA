---
title: Додавання та керування adminstrators-рекомендованими кроками
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: 142bf1474ac0e0eac5cecb9dddd35e28b6b6631e
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678867"
---
# <a name="how-to-add-and-manage-adminstrators---recommended-steps"></a><span data-ttu-id="a90e1-102">Додавання та керування adminstrators-рекомендованими кроками</span><span class="sxs-lookup"><span data-stu-id="a90e1-102">How to add and manage adminstrators - recommended steps</span></span>

<span data-ttu-id="a90e1-103">**Редагування адміністратора або Співадміністратора за передплатою**</span><span class="sxs-lookup"><span data-stu-id="a90e1-103">**Edit the Subscription Administrator or Co-administrator**</span></span>

- <span data-ttu-id="a90e1-104">Адміністратор облікового запису може редагувати обидві ролі, якщо адміністратор передплатникам може змінити лише один із адміністраторів на [порталі Azure](https://ms.portal.azure.com/#home).</span><span class="sxs-lookup"><span data-stu-id="a90e1-104">The Account Administrator can edit both roles whereas the Subscription Administrator can only change Co-administrators in the [Azure portal](https://ms.portal.azure.com/#home).</span></span>
- [<span data-ttu-id="a90e1-105">Додавання або змінення адміністраторів служби Azure передплатникам</span><span class="sxs-lookup"><span data-stu-id="a90e1-105">Add or change Azure subscription administrators</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

<span data-ttu-id="a90e1-106">**Оновлення адміністратора передплати або Co-Administrator для передплати на внутрішні (КОНДИЦІОНУВАННЯ)**</span><span class="sxs-lookup"><span data-stu-id="a90e1-106">**Update the Subscription Administrator or Co-Administrator for Internal (AIRS) Subscriptions**</span></span>

<span data-ttu-id="a90e1-107">Адміністратор служби або спільний адміністратор може самостійно обслуговувати цю дію, виконавши наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="a90e1-107">The Service Administrator or the Co-administrator can self-serve this action by using the following steps:</span></span>

1. <span data-ttu-id="a90e1-108">Увійдіть на [портал Azure](https://ms.portal.azure.com/#home) і клацніть елемент **керування витратами + виставлення рахунків** у лівому клинку.</span><span class="sxs-lookup"><span data-stu-id="a90e1-108">Log in to the [Azure portal](https://ms.portal.azure.com/#home) and click **Cost Management + Billing** in the left blade.</span></span>
2. <span data-ttu-id="a90e1-109">Клацніть елемент з передплатою.</span><span class="sxs-lookup"><span data-stu-id="a90e1-109">Click on the line item with your subscription.</span></span> <span data-ttu-id="a90e1-110">Відкриється огляд вашої передплатою.</span><span class="sxs-lookup"><span data-stu-id="a90e1-110">This opens the Overview for your subscription.</span></span>
3. <span data-ttu-id="a90e1-111">На клинку **передплатою** натисніть кнопку **Властивості**.</span><span class="sxs-lookup"><span data-stu-id="a90e1-111">On the **Subscription** blade, click **Properties**.</span></span> 
4. <span data-ttu-id="a90e1-112">Натисніть кнопку **адміністратор служби** .</span><span class="sxs-lookup"><span data-stu-id="a90e1-112">Click the **Service Admin** button.</span></span>
5. <span data-ttu-id="a90e1-113">Укажіть повідомлення електронної пошти користувача, якого потрібно встановити як адміністратор служби, і натисніть кнопку **OK**.</span><span class="sxs-lookup"><span data-stu-id="a90e1-113">Enter the email of the user whom you want to set as a Service Administrator and click **OK**.</span></span>

<span data-ttu-id="a90e1-114">**Додавання та змінення та видалення Співадміністратора**</span><span class="sxs-lookup"><span data-stu-id="a90e1-114">**Add/Change/Remove Co-administrator**</span></span>

1. <span data-ttu-id="a90e1-115">Увійдіть на портал " [Лазурний](https://ms.portal.azure.com/#home) " як адміністратор служби.</span><span class="sxs-lookup"><span data-stu-id="a90e1-115">Log in to the [Azure portal](https://ms.portal.azure.com/#home) as a Service Administrator.</span></span>
2. <span data-ttu-id="a90e1-116">Відкрийте [передплату та виберіть передплату.](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)</span><span class="sxs-lookup"><span data-stu-id="a90e1-116">Open [Subscriptions](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) and select a subscription.</span></span> <span data-ttu-id="a90e1-117">(Adminstrators можна призначати лише в області "Передплата".)</span><span class="sxs-lookup"><span data-stu-id="a90e1-117">(Co-adminstrators can only be assigned at the subscription scope.)</span></span>
3. <span data-ttu-id="a90e1-118">Перейдіть до **елемента керування доступом (IAM)**  >  **Classic адміністратори**  >  **додайте** елемент  >  **Додати** до адміністратора, щоб відкрити область **Додавання спільного адміністратора** (якщо параметр Add Co-адміністратор вимкнуто, це означає, що у вас немає дозволів).</span><span class="sxs-lookup"><span data-stu-id="a90e1-118">Navigate to **Access control (IAM)** > **Classic administrators** > **Add** > **Add co-administrator** to open the **Add co-admin** pane (If the Add co-administrator option is disabled, it denotes that you do not have permissions).</span></span>
4. <span data-ttu-id="a90e1-119">Виберіть користувача, якого потрібно додати, і натисніть кнопку **Додати**.</span><span class="sxs-lookup"><span data-stu-id="a90e1-119">Select the user whom you want to add and click **Add**.</span></span>

<span data-ttu-id="a90e1-120">**Дізнатися більше:**</span><span class="sxs-lookup"><span data-stu-id="a90e1-120">**Learn more:**</span></span>
- [<span data-ttu-id="a90e1-121">Додавання спільної адміністратора</span><span class="sxs-lookup"><span data-stu-id="a90e1-121">Add a Co-Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="a90e1-122">Видалення співадміністратора</span><span class="sxs-lookup"><span data-stu-id="a90e1-122">Remove a co-administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="a90e1-123">Змінення адміністратора служби</span><span class="sxs-lookup"><span data-stu-id="a90e1-123">Change the Service Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="a90e1-124">Перегляд адміністратора облікового запису</span><span class="sxs-lookup"><span data-stu-id="a90e1-124">View the Account Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="a90e1-125">Керування доступом за допомогою RBAC і Лазуропорталу</span><span class="sxs-lookup"><span data-stu-id="a90e1-125">Manage access using RBAC and Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

<span data-ttu-id="a90e1-126">**Додавання та видалення користувачів за допомогою служби Azure Active Directory (AD)**</span><span class="sxs-lookup"><span data-stu-id="a90e1-126">**Add/delete users using Azure Active Directory (AD)**</span></span>

<span data-ttu-id="a90e1-127">Ви можете додавати нових користувачів або видаляти вже доступні користувачі з організації Azure AD Active Directory:</span><span class="sxs-lookup"><span data-stu-id="a90e1-127">You can add new users or delete existing users from your Azure Active Directory (Azure AD) organization:</span></span>

1. <span data-ttu-id="a90e1-128">Щоб додати нового користувача, увійдіть на [портал Azure](https://ms.portal.azure.com/#home) , як адміністратор користувача для організації.</span><span class="sxs-lookup"><span data-stu-id="a90e1-128">To add a new user, log in to the [Azure portal](https://ms.portal.azure.com/#home) as a User-administrator for the organization.</span></span>
2. <span data-ttu-id="a90e1-129">Виберіть пункт " **Лазурний**", виберіть **користувачі** , а потім натисніть кнопку **створити користувача**.</span><span class="sxs-lookup"><span data-stu-id="a90e1-129">Select **Azure Active Directory**, select **Users** and then click **New user**.</span></span>
3. <span data-ttu-id="a90e1-130">На сторінці **користувача** заповніть необхідну інформацію.</span><span class="sxs-lookup"><span data-stu-id="a90e1-130">On the **User** page, fill out the required information.</span></span> <span data-ttu-id="a90e1-131">Натисніть кнопку **створити**.</span><span class="sxs-lookup"><span data-stu-id="a90e1-131">Click **Create**.</span></span> <span data-ttu-id="a90e1-132">Користувач створюється та додається до свого клієнта Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a90e1-132">The user is created and added to your Azure AD tenant.</span></span>

<span data-ttu-id="a90e1-133">**Додаткові відомості**:</span><span class="sxs-lookup"><span data-stu-id="a90e1-133">**Learn more**:</span></span>

- [<span data-ttu-id="a90e1-134">Додавання нового користувача</span><span class="sxs-lookup"><span data-stu-id="a90e1-134">Add a new user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="a90e1-135">Видалення користувача</span><span class="sxs-lookup"><span data-stu-id="a90e1-135">Delete a user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="a90e1-136">Додавання або оновлення відомостей профілю користувача за допомогою служби Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="a90e1-136">Add or update a user's profile information using Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

<span data-ttu-id="a90e1-137">**Рекомендовані документи**</span><span class="sxs-lookup"><span data-stu-id="a90e1-137">**Recommended documents**</span></span>

- [<span data-ttu-id="a90e1-138">Що таке елемент керування доступом на основі ролей (RBAC)?</span><span class="sxs-lookup"><span data-stu-id="a90e1-138">What is role-based access control (RBAC)?</span></span>](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [<span data-ttu-id="a90e1-139">Розуміння різних ролей у Azure</span><span class="sxs-lookup"><span data-stu-id="a90e1-139">Understand the different roles in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [<span data-ttu-id="a90e1-140">Дозволи на роль адміністратора в "Лазурний" Active Directory</span><span class="sxs-lookup"><span data-stu-id="a90e1-140">Administrator role permissions in Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [<span data-ttu-id="a90e1-141">Навчальний посібник: надання доступу для користувача за допомогою RBAC та порталу "Лазурний"</span><span class="sxs-lookup"><span data-stu-id="a90e1-141">Tutorial: Grant access for a user using RBAC and the Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [<span data-ttu-id="a90e1-142">Усунення несправностей у RBAC в лазуровий</span><span class="sxs-lookup"><span data-stu-id="a90e1-142">Troubleshoot RBAC in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [<span data-ttu-id="a90e1-143">Упорядкування ресурсів за допомогою «лазуровий груп керування»</span><span class="sxs-lookup"><span data-stu-id="a90e1-143">Organize your resources with Azure management groups</span></span>](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [<span data-ttu-id="a90e1-144">Запит на копіювання за допомогою електронної пошти копії Лазур-рахунка</span><span class="sxs-lookup"><span data-stu-id="a90e1-144">How to request copy of Azure invoice via email</span></span>](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [<span data-ttu-id="a90e1-145">Як додати, оновити або видалити кредитну або дебетову картку з Azure</span><span class="sxs-lookup"><span data-stu-id="a90e1-145">How to add, update or remove a credit or debit card from Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [<span data-ttu-id="a90e1-146">Керування (Повторна активація/скасування або переключення)</span><span class="sxs-lookup"><span data-stu-id="a90e1-146">Manage (Reactivate/Cancel/Switch) subscription</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



