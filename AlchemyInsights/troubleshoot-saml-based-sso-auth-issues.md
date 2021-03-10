---
title: Усунення несправностей із автентифікацією єдиного входу в SAML
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004341"
- "9409"
ms.openlocfilehash: c053e252edfcc51c95214c4bff4aded2bded2e23
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695663"
---
# <a name="troubleshoot-saml-based-sso-authentication-issues"></a><span data-ttu-id="3c4fd-102">Усунення несправностей із автентифікацією єдиного входу в SAML</span><span class="sxs-lookup"><span data-stu-id="3c4fd-102">Troubleshoot SAML-based SSO authentication issues</span></span>

<span data-ttu-id="3c4fd-103">Більшість користувачів можуть вирішувати проблеми автентифікації єдиного входу, виконавши такі Рекомендовані дії:</span><span class="sxs-lookup"><span data-stu-id="3c4fd-103">Most users are able to resolve their SAML-based SSO authentication issues using the following recommended steps:</span></span>

<span data-ttu-id="3c4fd-104">**Рекомендовані дії**</span><span class="sxs-lookup"><span data-stu-id="3c4fd-104">**Recommended Steps**</span></span>
1. <span data-ttu-id="3c4fd-105">Підстановка [поточних відомостей про код помилки](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#lookup-current-error-code-information).</span><span class="sxs-lookup"><span data-stu-id="3c4fd-105">Lookup [current error code information](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#lookup-current-error-code-information).</span></span>
1. <span data-ttu-id="3c4fd-106">Щоб вирішити помилки автентифікації, на [основі компонента "єдиний вхід" можна переглянути застосунки в Лазурому Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/debug-saml-sso-issues) .</span><span class="sxs-lookup"><span data-stu-id="3c4fd-106">See [Debug SAML-based single sign-on to applications in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/debug-saml-sso-issues) to resolve authentication errors.</span></span>
1. <span data-ttu-id="3c4fd-107">Щоб дізнатися про запити перевірки автентичності SAML 2,0 і відповідей, які Sign-On підтримуються в "Лазур" ("Лазурний"), зверніться до статті, що використовується в [одному Sign-On SAML](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol) .</span><span class="sxs-lookup"><span data-stu-id="3c4fd-107">Refer to the article, [Single Sign-On SAML protocol](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol) to learn about the SAML 2.0 authentication requests and responses that Azure Active Directory (Azure AD) supports for Single Sign-On (SSO).</span></span>


