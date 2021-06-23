---
title: Увімкнення автентифікації SMTP та виправлення неполадок
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
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077672"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a><span data-ttu-id="65784-102">Увімкнення автентифікації SMTP та виправлення неполадок</span><span class="sxs-lookup"><span data-stu-id="65784-102">Enable SMTP authentication and troubleshooting</span></span>

<span data-ttu-id="65784-103">Якщо потрібно активувати автентифікацію SMTP для поштової скриньки або ви отримуєте "Клієнт не автентифіковано", Помилка "Автентифікація невдала" або "SmtpClientAuthentication" з кодом 5.7.57 або 5.7.3 або 5.7.139 під час спроби надіслати повідомлення електронної пошти, автентифікацію пристрою або програми за допомогою Microsoft 365, щоб вирішити цю проблему, виконайте такі три дії:</span><span class="sxs-lookup"><span data-stu-id="65784-103">If you want to enable SMTP authentication for a mailbox or you're getting a "Client not authenticated", "Authentication unsuccessful", or "SmtpClientAuthentication" error with code 5.7.57 or 5.7.3 or 5.7.139 when you try to relay email by authenticating a device or application with Microsoft 365, perform these three actions to resolve the issue:</span></span>

1. <span data-ttu-id="65784-104">[Вимкніть стандартні параметри безпеки Azure,](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) установлювши перемикач **Увімкнути стандартні параметри безпеки** в значення **Ні.**</span><span class="sxs-lookup"><span data-stu-id="65784-104">Disable the [Azure security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) by toggling **Enable security defaults** to **No**.</span></span>

    <span data-ttu-id="65784-105">а.</span><span class="sxs-lookup"><span data-stu-id="65784-105">a.</span></span> <span data-ttu-id="65784-106">Увійдіть на портал Azure як адміністратор безпеки, адміністратор умовного доступу або глобальний адміністратор.</span><span class="sxs-lookup"><span data-stu-id="65784-106">Sign in to the Azure portal as a Security administrator, Conditional Access administrator, or global administrator.</span></span><BR/>
    <span data-ttu-id="65784-107">б.</span><span class="sxs-lookup"><span data-stu-id="65784-107">b.</span></span> <span data-ttu-id="65784-108">Перейдіть до Azure Active Directory > **Властивості.**</span><span class="sxs-lookup"><span data-stu-id="65784-108">Browse to Azure Active Directory > **Properties**.</span></span><BR/>
    <span data-ttu-id="65784-109">в.</span><span class="sxs-lookup"><span data-stu-id="65784-109">c.</span></span> <span data-ttu-id="65784-110">Виберіть **Елемент Керування параметрами безпеки за замовчуванням**.</span><span class="sxs-lookup"><span data-stu-id="65784-110">Select **Manage security defaults**.</span></span><BR/>
    <span data-ttu-id="65784-111">г.</span><span class="sxs-lookup"><span data-stu-id="65784-111">d.</span></span> <span data-ttu-id="65784-112">Установіть для **параметра Увімкнути безпеку за замовчуванням значення** **Ні**.</span><span class="sxs-lookup"><span data-stu-id="65784-112">Set **Enable security defaults** to **No**.</span></span><BR/>
    <span data-ttu-id="65784-113">е.</span><span class="sxs-lookup"><span data-stu-id="65784-113">e.</span></span> <span data-ttu-id="65784-114">Натисніть **кнопку Зберегти**.</span><span class="sxs-lookup"><span data-stu-id="65784-114">Select **Save**.</span></span>

2. <span data-ttu-id="65784-115">[Увімкніть надсилання SMTP клієнта](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) в ліцензованій поштовій скриньці.</span><span class="sxs-lookup"><span data-stu-id="65784-115">[Enable Client SMTP submission](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) on the licensed mailbox.</span></span>

    <span data-ttu-id="65784-116">а.</span><span class="sxs-lookup"><span data-stu-id="65784-116">a.</span></span> <span data-ttu-id="65784-117">У Центр адміністрування Microsoft 365 перейдіть до **пункту Активні** користувачі та виберіть користувача.</span><span class="sxs-lookup"><span data-stu-id="65784-117">From the Microsoft 365 admin center, go to **Active Users**, and select the user.</span></span><BR/>
    <span data-ttu-id="65784-118">б.</span><span class="sxs-lookup"><span data-stu-id="65784-118">b.</span></span> <span data-ttu-id="65784-119">Перейдіть на вкладку Пошта та в розділі Програми **електронної пошти** виберіть керування **програмами електронної пошти**.</span><span class="sxs-lookup"><span data-stu-id="65784-119">Go to Mail tab, and under **Email apps**, select **Manage email apps**.</span></span><BR/>
    <span data-ttu-id="65784-120">г.</span><span class="sxs-lookup"><span data-stu-id="65784-120">d.</span></span> <span data-ttu-id="65784-121">**Переконайтеся, що прапорець Автентифікований SMTP** (увімкнуто).</span><span class="sxs-lookup"><span data-stu-id="65784-121">Make sure **Authenticated SMTP** is checked (enabled).</span></span><BR/>
    <span data-ttu-id="65784-122">е.</span><span class="sxs-lookup"><span data-stu-id="65784-122">e.</span></span> <span data-ttu-id="65784-123">Виберіть **Save changes (Зберегти зміни).**</span><span class="sxs-lookup"><span data-stu-id="65784-123">Select **Save changes**.</span></span><BR/>

3. <span data-ttu-id="65784-124">[Вимкніть багатофакторну автентифікацію (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) у ліцензованій поштовій скриньці.</span><span class="sxs-lookup"><span data-stu-id="65784-124">[Disable Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) on the licensed mailbox.</span></span>

    <span data-ttu-id="65784-125">а.</span><span class="sxs-lookup"><span data-stu-id="65784-125">a.</span></span> <span data-ttu-id="65784-126">Перейдіть до меню Центр адміністрування Microsoft 365 в меню переходів ліворуч виберіть **Активні**  >  **користувачі.**</span><span class="sxs-lookup"><span data-stu-id="65784-126">Go to the Microsoft 365 admin center, and in the left navigation menu select **Users** > **Active users**.</span></span><BR/>
    <span data-ttu-id="65784-127">б.</span><span class="sxs-lookup"><span data-stu-id="65784-127">b.</span></span> <span data-ttu-id="65784-128">Виберіть **Багатофакторна автентифікація.**</span><span class="sxs-lookup"><span data-stu-id="65784-128">Select **Multi-factor authentication**.</span></span><BR/>
    <span data-ttu-id="65784-129">в.</span><span class="sxs-lookup"><span data-stu-id="65784-129">c.</span></span> <span data-ttu-id="65784-130">Виберіть користувача та **вимкніть multi-Factor auth.**</span><span class="sxs-lookup"><span data-stu-id="65784-130">Select the user and disable **Multi-Factor auth**.</span></span><BR/>
