---
title: Доступ до передплатою
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
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807726"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a><span data-ttu-id="3ea7a-102">Не вдається ввійти в Azure через проблеми з браузером (браузер зависає, продовжує обертатися, не завантажується і т. д.)</span><span class="sxs-lookup"><span data-stu-id="3ea7a-102">Unable to Sign-in Azure due to browser issues (Browser hangs, keeps spinning, does not load, etc.)</span></span>

<span data-ttu-id="3ea7a-103">Можливо, під час відключення ви можете зіткнутися.</span><span class="sxs-lookup"><span data-stu-id="3ea7a-103">You might be impacted by an outage.</span></span> <span data-ttu-id="3ea7a-104">Перевірте, чи є постійний процес відключення: « [блакитний стан здоров'я](https://status.azure.com/status/history/)».</span><span class="sxs-lookup"><span data-stu-id="3ea7a-104">Please check to see if there is an ongoing outage: [Azure Health Status](https://status.azure.com/status/history/).</span></span>

<span data-ttu-id="3ea7a-105">Вийдіть із усіх активних сесій Лазур.</span><span class="sxs-lookup"><span data-stu-id="3ea7a-105">Please log out of all the active Azure sessions.</span></span> <span data-ttu-id="3ea7a-106">Запустіть власний або режим анонімного перегляду веб-браузера.</span><span class="sxs-lookup"><span data-stu-id="3ea7a-106">Start a in-private or incognito mode of your web browser.</span></span>

<span data-ttu-id="3ea7a-107">Крім того, можна спробувати оновити браузер, використовувати інший браузер, видалити файли cookie кеша, якщо вище не працює.</span><span class="sxs-lookup"><span data-stu-id="3ea7a-107">You could also try to Refresh browser, use another browser, delete cache cookies if above doesn't work.</span></span>

<span data-ttu-id="3ea7a-108">Додаткові відомості: [усунення проблем із входом](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span><span class="sxs-lookup"><span data-stu-id="3ea7a-108">Learn more: [Troubleshoot Sign-in Issues](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span></span>

<span data-ttu-id="3ea7a-109">**Не вдається отримати доступ до передплати**</span><span class="sxs-lookup"><span data-stu-id="3ea7a-109">**Unable to access subscriptions**</span></span>

<span data-ttu-id="3ea7a-110">Переконайтеся, [що в полі "обліковий](https://portal.azure.com/)запис" у верхньому правому куті вибрано потрібний каталог "Лазурний".</span><span class="sxs-lookup"><span data-stu-id="3ea7a-110">In the [Azure portal](https://portal.azure.com/), make sure that the correct Azure directory is selected from the account at the top right.</span></span>

<span data-ttu-id="3ea7a-111">Переконайтеся, що для облікового запису, який використовується для адміністратора облікового запису, вибрано [пункт](https://account.windowsazure.com/Subscriptions)обліковий запис.</span><span class="sxs-lookup"><span data-stu-id="3ea7a-111">In the [Azure Account center](https://account.windowsazure.com/Subscriptions), make sure if the account used is the account admin.</span></span>

<span data-ttu-id="3ea7a-112">Додаткові відомості: [Виправлення неполадок із передплатою не знайдено](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="3ea7a-112">Learn more: [Troubleshoot No Subscriptions found](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="3ea7a-113">**Не вдається отримати доступ до журналу рахунків**</span><span class="sxs-lookup"><span data-stu-id="3ea7a-113">**Unable to access billing history**</span></span>

<span data-ttu-id="3ea7a-114">Адміністратор облікового запису повинен переконатися, що користувач, який має доступ до відомостей про виставлення рахунків, додається в "Блакитний Active Directory" як гостьовий користувач: [Додавання або видалення нового користувача](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="3ea7a-114">The account admin needs to make sure the user accessing the billing information is added in the Azure Active directory as a guest user: [Add or delete a new user](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="3ea7a-115">Користувач має надати роль глобального адміністратора: [призначити роль для користувачів](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="3ea7a-115">The user then needs to be given a Global admin role: [Assign role to users](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="3ea7a-116">Після цього користувач може надати доступ до рахунків за допомогою політики RBAC: [надати доступ до рахунків](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="3ea7a-116">Post this, the user can be given billing access using RBAC policies: [Grant access to billing](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="3ea7a-117">**Рекомендовані документи**</span><span class="sxs-lookup"><span data-stu-id="3ea7a-117">**Recommended Documents**</span></span>

-   [<span data-ttu-id="3ea7a-118">Я не можу ввійти, щоб керувати передплатою на Лазурне</span><span class="sxs-lookup"><span data-stu-id="3ea7a-118">I can't sign in to manage my Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)