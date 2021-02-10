---
title: Розгортання AD FS
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
- "1300012"
- "7420"
ms.openlocfilehash: a304504f7483036884878639dfa6ebfc3cdfcac8
ms.sourcegitcommit: 05a9dd3121c21322dc9ddec4c2eec548cafd5a43
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177712"
---
# <a name="deploy-ad-fs"></a><span data-ttu-id="865f5-102">Розгортання AD FS</span><span class="sxs-lookup"><span data-stu-id="865f5-102">Deploy AD FS</span></span>

<span data-ttu-id="865f5-103">Розгортання служб Федерації Active Directory (AD FS) використовує локальну інфраструктуру, щоб автентифікувати користувачів для служб Office 365.</span><span class="sxs-lookup"><span data-stu-id="865f5-103">An Active Directory Federation Services (AD FS) deployment uses your on-premises infrastructure to authenticate users for ‎Office 365 services.</span></span> <span data-ttu-id="865f5-104">За допомогою інтегрованого входу ви можете дозволити користувачам входити в Office 365 Services і програмне забезпечення як служби (SAAS), які інтегровані в Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="865f5-104">With federated sign-in, you can enable users to sign in to Office 365 services and Software as a Service (SAAS) applications that are integrated with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="865f5-105">Федеративні вхід засвідчує справжність користувачів від локального Active Directory за допомогою AD FS.</span><span class="sxs-lookup"><span data-stu-id="865f5-105">Federated sign-in authenticates users against your on-premises Active Directory via AD FS.</span></span> <span data-ttu-id="865f5-106">Крім того, під час корпоративної мережі користувачі не повинні вводити паролі повторно.</span><span class="sxs-lookup"><span data-stu-id="865f5-106">Also, while on the corporate network, users won't be required to reenter their passwords.</span></span>

<span data-ttu-id="865f5-107">[Порадник з розгортання AD FS](https://go.microsoft.com/fwlink/?linkid=2071178) надає покрокові вказівки з розгортання ЛОКАЛЬНОЇ ІНФРАСТРУКТУРИ AD FS, яка засвідчує справжність користувачів для служб Microsoft 365 і Office 365.</span><span class="sxs-lookup"><span data-stu-id="865f5-107">The [AD FS deployment advisor](https://go.microsoft.com/fwlink/?linkid=2071178) provides you with step-by-step guidance on deploying an on-premises AD FS infrastructure that authenticates users for Microsoft 365 and Office 365 services.</span></span> <span data-ttu-id="865f5-108">У цьому посібнику організація може переглядати компоненти та вимоги AD FS, придбавати та інсталювати сертифікати SSL, необхідні для розгортання, і інсталювати проксі-сервер необхідного веб-застосунку.</span><span class="sxs-lookup"><span data-stu-id="865f5-108">With this guide, your organization can review AD FS components and requirements, acquire and install SSL certificates that are necessary for deployment, and install a required web application proxy server.</span></span>
