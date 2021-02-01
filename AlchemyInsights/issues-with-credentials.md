---
title: Проблеми з обліковими даними
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
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063723"
---
# <a name="issues-with-credentials"></a><span data-ttu-id="e4ae1-102">Проблеми з обліковими даними</span><span class="sxs-lookup"><span data-stu-id="e4ae1-102">Issues with credentials</span></span>

<span data-ttu-id="e4ae1-103">Програма [ідентифікації клієнтів Microsoft і потік облікових даних клієнта "oauth 2,0"](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) описує, як можна програмувати безпосередньо в разі надання відповідного потоку облікових даних клієнтів oauth 2,0.</span><span class="sxs-lookup"><span data-stu-id="e4ae1-103">[Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describes how to program directly against the OAuth 2.0 client credentials grant flow.</span></span>

<span data-ttu-id="e4ae1-104">**Як керувати паролем або обліковими даними програми?**</span><span class="sxs-lookup"><span data-stu-id="e4ae1-104">**How do I manage an application's password or certificate credentials?**</span></span>

<span data-ttu-id="e4ae1-105">У лазуровий CLI, ви можете використовувати [облікові дані застосунку з оголошеннями](https://docs.microsoft.com/cli/azure/ad/app/credential) , щоб видалити, список або скинути пароль програми або облікові дані сертифіката.</span><span class="sxs-lookup"><span data-stu-id="e4ae1-105">In the Azure CLI, you can use [az ad app credential](https://docs.microsoft.com/cli/azure/ad/app/credential) to delete, list, or reset an application's password or certificate credentials.</span></span>

<span data-ttu-id="e4ae1-106">**Як користувачі скине свої паролі?**</span><span class="sxs-lookup"><span data-stu-id="e4ae1-106">**How do my users reset their passwords?**</span></span>

<span data-ttu-id="e4ae1-107">Користувачам потрібно [зареєструватися для автоматичного скидання пароля](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) , перш ніж вони зможуть скинути паролі.</span><span class="sxs-lookup"><span data-stu-id="e4ae1-107">Users need to [register for self-service password reset](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) before they can reset their passwords.</span></span> <span data-ttu-id="e4ae1-108">Зареєструвавши користувача, ви можете виконати вказівки, описані в цій статті, щоб скинути пароль: [скидання робочого або навчального пароля](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span><span class="sxs-lookup"><span data-stu-id="e4ae1-108">Once a user has registered, they can follow the instructions in this article to reset their password: [Reset your work or school password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span></span>

<span data-ttu-id="e4ae1-109">**Як користувачі змінюють свої паролі?**</span><span class="sxs-lookup"><span data-stu-id="e4ae1-109">**How do my users change their passwords?**</span></span>

<span data-ttu-id="e4ae1-110">Користувачі можуть виконувати кроки, описані в цій статті, щоб змінити їхні паролі: [як змінити пароль](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span><span class="sxs-lookup"><span data-stu-id="e4ae1-110">Users can follow the steps in this article to change their passwords: [How to change your password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span></span>
<span data-ttu-id="e4ae1-111">Вони також можуть [керувати паролями програм для двоетапної перевірки](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span><span class="sxs-lookup"><span data-stu-id="e4ae1-111">They can also [Manage app passwords for two-step verification](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span></span>

<span data-ttu-id="e4ae1-112">**Під час змінення або скидання пароля в користувача з'являється повідомлення про помилку**</span><span class="sxs-lookup"><span data-stu-id="e4ae1-112">**My user is getting an error when changing or resetting their password**</span></span>

<span data-ttu-id="e4ae1-113">Це посилання надасть інформацію про поширені проблеми, які можуть виникати, коли користувач намагається скинути пароль: [поширені проблеми та їхні рішення](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span><span class="sxs-lookup"><span data-stu-id="e4ae1-113">This link will provide information on common problems that can arise when a user is trying to reset their password: [Common problems and their solutions](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span></span>

<span data-ttu-id="e4ae1-114">**Помилка скидання пароля користувача**</span><span class="sxs-lookup"><span data-stu-id="e4ae1-114">**I'm having a problem resetting a user's password**</span></span>

- <span data-ttu-id="e4ae1-115">Переконайтеся, що ви авторизовані для скидання паролів.</span><span class="sxs-lookup"><span data-stu-id="e4ae1-115">Make sure you are authorized to reset passwords.</span></span> <span data-ttu-id="e4ae1-116">*Скинути паролі користувачів можна лише за глобальними, паролем і адміністраторами користувачів.*</span><span class="sxs-lookup"><span data-stu-id="e4ae1-116">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="e4ae1-117">Глобальні адміністратори також можуть скинути паролі іншого привілейованого адміністратора.</span><span class="sxs-lookup"><span data-stu-id="e4ae1-117">Global administrators can also reset other privileged administrator's passwords.</span></span>

- <span data-ttu-id="e4ae1-118">Переконайтеся, що ви зрозуміли вимоги до ліцензування:</span><span class="sxs-lookup"><span data-stu-id="e4ae1-118">Make sure you understand the licensing requirements:</span></span>

  - <span data-ttu-id="e4ae1-119">У вашій організації має бути принаймні одну ліцензію.</span><span class="sxs-lookup"><span data-stu-id="e4ae1-119">You must have at least one license assigned in your organization:</span></span>
    - <span data-ttu-id="e4ae1-120">**Хмарні тільки користувачі** – будь-який Office 365 (O365) платний обліковий номер або ЛАЗУРНЕ AD Basic</span><span class="sxs-lookup"><span data-stu-id="e4ae1-120">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="e4ae1-121">**Хмарні та/або Локальні користувачі** – AZURE AD Premium P1 або P2, Enterprise Mobility + Security (EMS) або захищене продуктивне підприємство (SPE).</span><span class="sxs-lookup"><span data-stu-id="e4ae1-121">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="e4ae1-122">Докладні відомості про вимоги до ліцензування наведено в статті [вимоги до ліцензування для скидання пароля служби самообслуговування Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span><span class="sxs-lookup"><span data-stu-id="e4ae1-122">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span></span>
- <span data-ttu-id="e4ae1-123">Щоб скинути пароль користувача, виберіть користувача в Лазур.</span><span class="sxs-lookup"><span data-stu-id="e4ae1-123">To reset a user's password, find the user in Azure AD.</span></span> <span data-ttu-id="e4ae1-124">Потім у полі огляд для цього користувача натисніть кнопку "скинути пароль".</span><span class="sxs-lookup"><span data-stu-id="e4ae1-124">Then, on the overview blade for that user, click the "reset password" button.</span></span>

<span data-ttu-id="e4ae1-125">**Кнопка "скидання пароля"**</span><span class="sxs-lookup"><span data-stu-id="e4ae1-125">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="e4ae1-126">Ви не авторизовані для скидання паролів **цього** користувача.</span><span class="sxs-lookup"><span data-stu-id="e4ae1-126">You are not authorized to reset **this** user's passwords.</span></span> <span data-ttu-id="e4ae1-127">*Скинути паролі користувачів можна лише за глобальними, паролем і адміністраторами користувачів.*</span><span class="sxs-lookup"><span data-stu-id="e4ae1-127">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="e4ae1-128">Глобальні адміністратори також можуть скинути паролі іншого привілейованого адміністратора.</span><span class="sxs-lookup"><span data-stu-id="e4ae1-128">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="e4ae1-129">**Не відображається лезо скидання пароля**</span><span class="sxs-lookup"><span data-stu-id="e4ae1-129">**I don't see the password reset blade**</span></span>

<span data-ttu-id="e4ae1-130">Ви не авторизовані для скидання паролів.</span><span class="sxs-lookup"><span data-stu-id="e4ae1-130">You are not authorized to reset passwords.</span></span> <span data-ttu-id="e4ae1-131">*Скинути паролі користувачів можна лише за глобальними, паролем і адміністраторами користувачів.*</span><span class="sxs-lookup"><span data-stu-id="e4ae1-131">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="e4ae1-132">Глобальні адміністратори також можуть скинути паролі іншого привілейованого адміністратора.</span><span class="sxs-lookup"><span data-stu-id="e4ae1-132">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="e4ae1-133">**У разі скидання пароля не відображається локальна відповідь для інтеграції**</span><span class="sxs-lookup"><span data-stu-id="e4ae1-133">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="e4ae1-134">Локальна відповідь на інтеграцію відображається лише в гібридних середовищах – тобто ви використовуєте перезапису пароля, щоб маніпулювати паролями локального користувача.</span><span class="sxs-lookup"><span data-stu-id="e4ae1-134">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>

- <span data-ttu-id="e4ae1-135">Цей Клинок не відображається, якщо:</span><span class="sxs-lookup"><span data-stu-id="e4ae1-135">You do not see this blade if:</span></span>

  - <span data-ttu-id="e4ae1-136">Ви не використовуєте wriтиback пароля</span><span class="sxs-lookup"><span data-stu-id="e4ae1-136">You are not using password writeback</span></span>
  - <span data-ttu-id="e4ae1-137">Виникла проблема з інсталяцією та підключенням облікового запису для wriadback</span><span class="sxs-lookup"><span data-stu-id="e4ae1-137">There is a problem with your installation/connectivity of password writeback</span></span>
  - <span data-ttu-id="e4ae1-138">Виникла проблема з інсталяцією та підключенням служби Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="e4ae1-138">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
  - <span data-ttu-id="e4ae1-139">Додаткові кроки з виправлення неполадок, які допоможуть вирішити проблему з wriтиповернення пароля, перегляньте статтю [Виправлення неполадок із wrileback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="e4ae1-139">For more troubleshooting steps for issues with password writeback, see [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span></span>

<span data-ttu-id="e4ae1-140">**Я не знаю, як скинути пароль користувача**</span><span class="sxs-lookup"><span data-stu-id="e4ae1-140">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="e4ae1-141">Увійдіть на портал "Лазурний" як відповідний адміністратор.</span><span class="sxs-lookup"><span data-stu-id="e4ae1-141">Sign in to the Azure portal as an appropriate admin.</span></span>
2. <span data-ttu-id="e4ae1-142">Перейдіть до леза " **користувачі та групи** ", виберіть **усі користувачі**.</span><span class="sxs-lookup"><span data-stu-id="e4ae1-142">Go to the **Users and groups** blade, select **All Users**.</span></span>
3. <span data-ttu-id="e4ae1-143">Виберіть користувача зі списку.</span><span class="sxs-lookup"><span data-stu-id="e4ae1-143">Select a user from the list.</span></span>
4. <span data-ttu-id="e4ae1-144">Для вибраного користувача виберіть **Огляд**, а потім на панелі команд натисніть кнопку **скинути пароль**.</span><span class="sxs-lookup"><span data-stu-id="e4ae1-144">For the selected user, select **Overview**, and then in the command bar, select **Reset password**.</span></span>
5. <span data-ttu-id="e4ae1-145">Натисніть кнопку **скидання пароля** та дотримуйтеся вказівок на екрані.</span><span class="sxs-lookup"><span data-stu-id="e4ae1-145">Select the **Reset password** button and follow the instructions on the screen.</span></span>
    - <span data-ttu-id="e4ae1-146">Тільки скидання **здійснюється за допомогою** облікового запису "wrireback".</span><span class="sxs-lookup"><span data-stu-id="e4ae1-146">Only resets performed through the **Azure portal** support password writeback.</span></span>

<span data-ttu-id="e4ae1-147">**Я скину пароль локального користувача з порталу адміністрування Office 365 або Office 365 для мобільних пристроїв, але користувач все ще не зможе ввійти**</span><span class="sxs-lookup"><span data-stu-id="e4ae1-147">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="e4ae1-148">На цьому порталі не підтримується Wriтиповернення пароля.</span><span class="sxs-lookup"><span data-stu-id="e4ae1-148">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="e4ae1-149">Знову скиньте пароль користувача на порталі Azure.</span><span class="sxs-lookup"><span data-stu-id="e4ae1-149">Reset the user's password again in the Azure portal.</span></span>
