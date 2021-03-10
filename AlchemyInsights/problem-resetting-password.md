---
title: Помилка скидання пароля
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696282"
---
# <a name="problems-resetting-password"></a><span data-ttu-id="94aa2-102">Проблеми з відновленням пароля</span><span class="sxs-lookup"><span data-stu-id="94aa2-102">Problems resetting password</span></span>

<span data-ttu-id="94aa2-103">Нижче наведено деякі з проблем, які можуть виникнути під час скидання пароля та можливих рішень.</span><span class="sxs-lookup"><span data-stu-id="94aa2-103">Following are some of the issues that you might face when resetting password and the possible solutions:</span></span>

<span data-ttu-id="94aa2-104">**У мене виникла проблема з скидлення пароля, не охоплених іншими категоріями**</span><span class="sxs-lookup"><span data-stu-id="94aa2-104">**I'm having an issue with password reset not covered in the other categories**</span></span>

- <span data-ttu-id="94aa2-105">Переконайтеся, що ви авторизовані для скидання паролів.</span><span class="sxs-lookup"><span data-stu-id="94aa2-105">Ensure you are authorized to reset passwords.</span></span> <span data-ttu-id="94aa2-106">Скинути паролі користувачів можна лише за глобальними, паролем і адміністраторами користувачів.</span><span class="sxs-lookup"><span data-stu-id="94aa2-106">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="94aa2-107">Глобальні адміністратори також можуть скинути паролі іншого привілейованого адміністратора.</span><span class="sxs-lookup"><span data-stu-id="94aa2-107">Global administrators can also reset other privileged administrator's passwords.</span></span>
- <span data-ttu-id="94aa2-108">Переконайтеся, що ви розумієте вимоги до ліцензування:</span><span class="sxs-lookup"><span data-stu-id="94aa2-108">Ensure that you understand the licensing requirements:</span></span>
    - <span data-ttu-id="94aa2-109">Потрібно мати принаймні одну ліцензію, призначену в організації</span><span class="sxs-lookup"><span data-stu-id="94aa2-109">You must have at least one license assigned in your organization</span></span>
        - <span data-ttu-id="94aa2-110">Хмарні тільки користувачі – будь-який Office 365 (O365) платний ОБЛІКОВИЙ номер або Лазурне AD Basic</span><span class="sxs-lookup"><span data-stu-id="94aa2-110">Cloud only users - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
        - <span data-ttu-id="94aa2-111">Хмарні та/або Локальні користувачі – Azure AD Premium P1 або P2, Enterprise Mobility + Security (EMS) або захищене продуктивне підприємство (SPE).</span><span class="sxs-lookup"><span data-stu-id="94aa2-111">Cloud and/or on-premises users - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
        - <span data-ttu-id="94aa2-112">Додаткові відомості про вимоги до ліцензування наведено в статті [вимоги до ліцензування для неавтоматичного скидання пароля служби "Лазурний](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)".</span><span class="sxs-lookup"><span data-stu-id="94aa2-112">To read more about licensing requirements see the article [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="94aa2-113">**Утруднення під час перевірки політики скидання пароля**</span><span class="sxs-lookup"><span data-stu-id="94aa2-113">**I'm having problems testing the password reset policy I set**</span></span>

- <span data-ttu-id="94aa2-114">Нещодавно застосовані політики можуть виконувати кілька хвилин, щоб реплікувати всі центри даних і кінцеві точки.</span><span class="sxs-lookup"><span data-stu-id="94aa2-114">Recently applied policies can take several minutes to replicate across all data centers and end-points.</span></span> <span data-ttu-id="94aa2-115">Фізична відстань від центру обробки даних також вплине на спосіб застосування швидко внесених змін.</span><span class="sxs-lookup"><span data-stu-id="94aa2-115">Physical distance from the data center will also affect how quickly changes are applied.</span></span>
- <span data-ttu-id="94aa2-116">Перевірка з кінцевим користувачем, а не адміністратором і пілотом з невеликим набором користувачів.</span><span class="sxs-lookup"><span data-stu-id="94aa2-116">Test with an end user, not an administrator, and pilot with a small set of users.</span></span> <span data-ttu-id="94aa2-117">Політики, настроєні на порталі "Лазурний", призначено лише кінцевим користувачам, а не адміністраторам.</span><span class="sxs-lookup"><span data-stu-id="94aa2-117">The policies configured in the Azure portal ONLY apply to end-users, not administrators.</span></span> <span data-ttu-id="94aa2-118">Корпорація Майкрософт застосовує сильну політику скидання пароля за два ворота для будь-якого роль (приклад: Глобальний адміністратор, адміністратор служби підтримки, адміністратор паролів тощо).</span><span class="sxs-lookup"><span data-stu-id="94aa2-118">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role (Example: Global Administrator, Helpdesk Administrator, Password Administrator, etc.)</span></span>
    - <span data-ttu-id="94aa2-119">Дізнайтеся більше про [політики для адміністраторів](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span><span class="sxs-lookup"><span data-stu-id="94aa2-119">Learn more about [policies for administrators](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span></span>

<span data-ttu-id="94aa2-120">**Я хочу розгорнути скидання пароля, але я не хочу, щоб мої користувачі реєструватимемо додаткові відомості про безпеку**</span><span class="sxs-lookup"><span data-stu-id="94aa2-120">**I want to deploy password reset but I don't want to make my users register additional security info**</span></span>

<span data-ttu-id="94aa2-121">Попередньо заповніть дані для користувачів, щоб їх не було!</span><span class="sxs-lookup"><span data-stu-id="94aa2-121">Pre-populate data for your users so they don't have to!</span></span> <span data-ttu-id="94aa2-122">-Адміністратор дає змогу налаштувати параметри телефону та електронної пошти для користувачів, перш ніж установлювати скидання пароля до вашої організації.</span><span class="sxs-lookup"><span data-stu-id="94aa2-122">- As an administrator you can set phone and email properties for your users before rolling out password reset to your organization.</span></span> <span data-ttu-id="94aa2-123">Ви можете зробити це за допомогою API, PowerShell або Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="94aa2-123">You can do this using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="94aa2-124">Додаткові відомості тут:</span><span class="sxs-lookup"><span data-stu-id="94aa2-124">More information here:</span></span>
- [<span data-ttu-id="94aa2-125">Розгортання скидання пароля без необхідності реєструвати користувачів</span><span class="sxs-lookup"><span data-stu-id="94aa2-125">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [<span data-ttu-id="94aa2-126">Дані, які використовуються для скидання пароля</span><span class="sxs-lookup"><span data-stu-id="94aa2-126">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="94aa2-127">**Кнопка "скидання пароля"**</span><span class="sxs-lookup"><span data-stu-id="94aa2-127">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="94aa2-128">Ви не авторизовані для скидання паролів цього користувача.</span><span class="sxs-lookup"><span data-stu-id="94aa2-128">You are not authorized to reset this user's passwords.</span></span> <span data-ttu-id="94aa2-129">Скинути паролі користувачів можна лише за глобальними, паролем і адміністраторами користувачів.</span><span class="sxs-lookup"><span data-stu-id="94aa2-129">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="94aa2-130">Глобальні адміністратори також можуть скинути паролі іншого привілейованого адміністратора.</span><span class="sxs-lookup"><span data-stu-id="94aa2-130">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="94aa2-131">**Не відображається лезо скидання пароля**</span><span class="sxs-lookup"><span data-stu-id="94aa2-131">**I don't see the password reset blade**</span></span>

<span data-ttu-id="94aa2-132">Ви не авторизовані для скидання паролів.</span><span class="sxs-lookup"><span data-stu-id="94aa2-132">You are not authorized to reset passwords.</span></span> <span data-ttu-id="94aa2-133">Скинути паролі користувачів можна лише за глобальними, паролем і адміністраторами користувачів.</span><span class="sxs-lookup"><span data-stu-id="94aa2-133">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="94aa2-134">Глобальні адміністратори також можуть скинути паролі іншого привілейованого адміністратора.</span><span class="sxs-lookup"><span data-stu-id="94aa2-134">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="94aa2-135">**У разі скидання пароля не відображається локальна відповідь для інтеграції**</span><span class="sxs-lookup"><span data-stu-id="94aa2-135">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="94aa2-136">Локальна відповідь на інтеграцію відображається лише в гібридних середовищах – тобто ви використовуєте перезапису пароля, щоб маніпулювати паролями локального користувача.</span><span class="sxs-lookup"><span data-stu-id="94aa2-136">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>
- <span data-ttu-id="94aa2-137">Цей Клинок не відображається, якщо:</span><span class="sxs-lookup"><span data-stu-id="94aa2-137">You do not see this blade if:</span></span>
    - <span data-ttu-id="94aa2-138">Ви не використовуєте wriтиback пароля</span><span class="sxs-lookup"><span data-stu-id="94aa2-138">You are not using password writeback</span></span>
    - <span data-ttu-id="94aa2-139">Виникла проблема з інсталяцією та підключенням облікового запису для wriadback</span><span class="sxs-lookup"><span data-stu-id="94aa2-139">There is a problem with your installation/connectivity of password writeback</span></span>
    - <span data-ttu-id="94aa2-140">Виникла проблема з інсталяцією та підключенням служби Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="94aa2-140">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
    - <span data-ttu-id="94aa2-141">Додаткові кроки з виправлення неполадок, які допоможуть вирішити проблему з wriseback, ознайомтеся з розділом [Виправлення неполадок із wriseback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="94aa2-141">For more troubleshooting steps for issues with password writeback, see the section [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="94aa2-142">**Я не знаю, як скинути пароль користувача**</span><span class="sxs-lookup"><span data-stu-id="94aa2-142">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="94aa2-143">Увійдіть на портал "Лазурний" як відповідний адміністратор.</span><span class="sxs-lookup"><span data-stu-id="94aa2-143">Sign in to the Azure portal as an appropriate admin.</span></span>
1. <span data-ttu-id="94aa2-144">Перейдіть до леза "користувачі та групи", виберіть **усі користувачі**.</span><span class="sxs-lookup"><span data-stu-id="94aa2-144">Go to the Users and groups blade, select **All Users**.</span></span>
1. <span data-ttu-id="94aa2-145">Виберіть користувача зі списку.</span><span class="sxs-lookup"><span data-stu-id="94aa2-145">Select a user from the list.</span></span>
1. <span data-ttu-id="94aa2-146">Для вибраного користувача виберіть **Огляд**, а потім на панелі команд натисніть кнопку **скинути пароль**.</span><span class="sxs-lookup"><span data-stu-id="94aa2-146">For the selected user, select **Overview**, and then in the command bar, click **Reset password**.</span></span>
1. <span data-ttu-id="94aa2-147">Дотримуйтеся вказівок на екрані.</span><span class="sxs-lookup"><span data-stu-id="94aa2-147">Follow the instructions on the screen.</span></span>
    - <span data-ttu-id="94aa2-148">Тільки скидання здійснюється за допомогою облікового запису "wrireback".</span><span class="sxs-lookup"><span data-stu-id="94aa2-148">Only resets performed through the Azure portal support password writeback.</span></span>

<span data-ttu-id="94aa2-149">**Я скину пароль локального користувача з порталу адміністрування Office 365 або Office 365 для мобільних пристроїв, але користувач все ще не зможе ввійти**</span><span class="sxs-lookup"><span data-stu-id="94aa2-149">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="94aa2-150">На цьому порталі не підтримується Wriтиповернення пароля.</span><span class="sxs-lookup"><span data-stu-id="94aa2-150">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="94aa2-151">Знову скиньте пароль користувача на порталі Azure-portal.azure.com</span><span class="sxs-lookup"><span data-stu-id="94aa2-151">Reset the user's password again in the Azure portal - portal.azure.com</span></span>

