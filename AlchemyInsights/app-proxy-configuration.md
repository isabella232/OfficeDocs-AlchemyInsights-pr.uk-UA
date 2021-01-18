---
title: Конфігурація проксі-сервера програми
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
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885532"
---
# <a name="app-proxy-configuration"></a><span data-ttu-id="c5675-102">Конфігурація проксі-сервера програми</span><span class="sxs-lookup"><span data-stu-id="c5675-102">App Proxy Configuration</span></span>

1. <span data-ttu-id="c5675-103">Щоб дізнатися, як настроїти програму проксі-сервера застосунку в поданні Azure AD, щоб відобразити локальні програми в хмарі, Дізнайтеся, [як настроїти програму проксі-застосунку програми](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span><span class="sxs-lookup"><span data-stu-id="c5675-103">To understand how to configure an Application Proxy application within Azure AD to expose your on-premises applications to the cloud, see [How to configure an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span></span>
2. <span data-ttu-id="c5675-104">Єдиний вхід (SSO) дає змогу користувачам отримувати доступ до програми без автентифікації кілька разів.</span><span class="sxs-lookup"><span data-stu-id="c5675-104">Single sign-on (SSO) allows your users to access an application without authenticating multiple times.</span></span> <span data-ttu-id="c5675-105">Ця функція дає змогу виконати одну автентифікацію в хмарі, у порівнянні з Azure Active Directory, і дозволяє службі або сполучну лінію, щоб видати користувачу можливість виконувати додаткові проблеми з автентифікацією в програмі.</span><span class="sxs-lookup"><span data-stu-id="c5675-105">It allows the single authentication to occur in the cloud, against Azure Active Directory, and allows the service or Connector to impersonate the user to complete any additional authentication challenges from the application.</span></span> <span data-ttu-id="c5675-106">Щоб дізнатися більше, Дізнайтеся, [як настроїти єдиний вхід у програму проксі-сервера застосунку](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span><span class="sxs-lookup"><span data-stu-id="c5675-106">To learn more, see [How to configure single sign-on to an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span></span>
3. <span data-ttu-id="c5675-107">[Ця стаття](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) використовується для усунення поширених проблем, які виникають під час створення нової програми проксі-застосунку.</span><span class="sxs-lookup"><span data-stu-id="c5675-107">Use [this article](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) to troubleshoot common issues people face when creating a new application proxy application.</span></span>
4. <span data-ttu-id="c5675-108">Якщо у вас виникли проблеми з настроюванням автентифікації на основі цієї програми, можливо, знадобиться [виправити конфігурацію для проксі-сервера Kerberos](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) , щоб вирішити цю проблему, або вказівки з [Настроювання програми за допомогою pingaccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) .</span><span class="sxs-lookup"><span data-stu-id="c5675-108">If you are having a problem setting up back-end authentication to your application you may need to [Troubleshoot Kerberos constrained delegation configurations for Application Proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) or follow guidance on [configuring application with PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) to resolve your issue.</span></span>
