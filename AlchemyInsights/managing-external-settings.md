---
title: Керування зовнішніми настройками
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: 7caf46f9988ddbcbb16c0a2751dbda85bd7da34c
ms.sourcegitcommit: 616ae0cbd5769e12ae428e00088840cf05e52b6a
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/17/2021
ms.locfileid: "50294429"
---
# <a name="managing-external-settings"></a><span data-ttu-id="f87bf-102">Керування зовнішніми настройками</span><span class="sxs-lookup"><span data-stu-id="f87bf-102">Managing External Settings</span></span>

<span data-ttu-id="f87bf-103">**Оголошення**</span><span class="sxs-lookup"><span data-stu-id="f87bf-103">**Announcement**</span></span>

- <span data-ttu-id="f87bf-104">[Припинення роботи входу в WebView від Google починаючи з 4 січня 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span><span class="sxs-lookup"><span data-stu-id="f87bf-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span></span> <span data-ttu-id="f87bf-105">Перевірте, чи впливають ваші програми, дотримуючись вказівок Google на сумісність із тестуваннями</span><span class="sxs-lookup"><span data-stu-id="f87bf-105">Test whether your apps are affected by following Google’s guidance on testing compatibility</span></span>
- <span data-ttu-id="f87bf-106">Переконайтеся, що під час входу в обліковий запис користувача з обліковими записами користувачів Google можна використовувати системну веб-подання або системний браузер.</span><span class="sxs-lookup"><span data-stu-id="f87bf-106">Make sure to use the system webview or the system browser when signing in your users with consumer Google accounts</span></span>

<span data-ttu-id="f87bf-107">**Керування настройками запрошень**</span><span class="sxs-lookup"><span data-stu-id="f87bf-107">**Manage Invitation Settings**</span></span>

<span data-ttu-id="f87bf-108">Переконайтеся, що ви [налаштували параметри зовнішньої співпраці](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) , щоб надати відповідним користувачам можливість отримувати запрошення.</span><span class="sxs-lookup"><span data-stu-id="f87bf-108">Confirm that you have [configured the external collaboration settings](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) to allow the appropriate people to send invitations.</span></span>

<span data-ttu-id="f87bf-109">**Керування дозволами на доступ для гостьових користувачів**</span><span class="sxs-lookup"><span data-stu-id="f87bf-109">**Manage Guest User Access Permissions**</span></span>

1. <span data-ttu-id="f87bf-110">Глобальні адміністратори можуть керувати дозволами гостьового доступу в каталозі за допомогою порталу "Лазурний", настроївши дозволи на доступ до гостьового доступу на сторінці "Параметри зовнішньої співпраці".</span><span class="sxs-lookup"><span data-stu-id="f87bf-110">Global admins can manage guest access permissions in the directory through the Azure portal by configuring the guest access permissions on the External Collaboration Settings page.</span></span> <span data-ttu-id="f87bf-111">[Дізнайтеся більше про цей параметр](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="f87bf-111">[Learn more about this setting](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
2. <span data-ttu-id="f87bf-112">Якщо ви хочете, щоб ваші гості могли отримати доступ до таких програм, як команди або SharePoint, переконайтеся, що ці застосунки настроєно для надання доступу за Гостьовим доступом.</span><span class="sxs-lookup"><span data-stu-id="f87bf-112">If you would like your guests to access apps such as Teams or SharePoint, confirm that you've configured those apps to allow guest access.</span></span> <span data-ttu-id="f87bf-113">Дізнайтеся більше про [настройки команд](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) і [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="f87bf-113">Learn more about the [Teams settings](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) and [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="f87bf-114">**Настроювання запрошень:**</span><span class="sxs-lookup"><span data-stu-id="f87bf-114">**Configuring invitations:**</span></span>

- [<span data-ttu-id="f87bf-115">Активація B2B зовнішньої співпраці та керування користувачами, які можуть запросити гостей</span><span class="sxs-lookup"><span data-stu-id="f87bf-115">Enable B2B external collaboration and manage who can invite guests</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="f87bf-116">Дозволити або заблокувати запрошення для користувачів із певних організацій</span><span class="sxs-lookup"><span data-stu-id="f87bf-116">Allow or block invitations to users from specific organizations</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="f87bf-117">**Настроювання дозволених постачальників посвідчень:**</span><span class="sxs-lookup"><span data-stu-id="f87bf-117">**Configuring allowed identity providers:**</span></span>

- [<span data-ttu-id="f87bf-118">Федерація Google</span><span class="sxs-lookup"><span data-stu-id="f87bf-118">Google Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="f87bf-119">Пряма Федерація</span><span class="sxs-lookup"><span data-stu-id="f87bf-119">Direct Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="f87bf-120">Автентифікація за один раз для електронної пошти</span><span class="sxs-lookup"><span data-stu-id="f87bf-120">Email one-time Passcode Authentication</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
