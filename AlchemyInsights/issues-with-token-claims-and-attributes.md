---
title: Проблеми з відповідними вимогами і атрибутами маркерів
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
- "9004347"
- "7761"
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/27/2021
ms.locfileid: "50036081"
---
# <a name="issues-with-token-claims-and-attributes"></a><span data-ttu-id="64359-102">Проблеми з відповідними вимогами і атрибутами маркерів</span><span class="sxs-lookup"><span data-stu-id="64359-102">Issues with Token Claims and Attributes</span></span>

<span data-ttu-id="64359-103">**Оновлення, настроювання та видалення тверджень про маркер**</span><span class="sxs-lookup"><span data-stu-id="64359-103">**Update, configure or remove token claims**</span></span>

1. <span data-ttu-id="64359-104">Використовуючи Azure Active Directory (Azure AD), можна [Настроїти тип твердження для твердження про роль](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) у відповіді, який ви отримали після авторизації програми.</span><span class="sxs-lookup"><span data-stu-id="64359-104">By using Azure Active Directory (Azure AD), you can [customize the claim type for the role claim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) in the response token that you receive after you authorize an app.</span></span>
2. <span data-ttu-id="64359-105">Розробники програм можуть використовувати необов'язкові претензії в своїх програмах Azure AD, щоб указати, які претензії вони хочуть в маркери, які надходять до їх програми.</span><span class="sxs-lookup"><span data-stu-id="64359-105">Application developers can use optional claims in their Azure AD applications to specify which claims they want in tokens sent to their application.</span></span> <span data-ttu-id="64359-106">Додаткові відомості наведено в статті [надання необов'язкових претензій до програми](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span><span class="sxs-lookup"><span data-stu-id="64359-106">For more information, see [Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span></span>
3. <span data-ttu-id="64359-107">[Настройте вимоги до груп для програм за допомогою служби Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span><span class="sxs-lookup"><span data-stu-id="64359-107">[Configure group claims for applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span></span>
4. <span data-ttu-id="64359-108">Якщо у вашій програмі використовується небезшовний єдиний вхід, див. розділ ["настроїти претензії, видані в маркер SAML для корпоративних програм"](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span><span class="sxs-lookup"><span data-stu-id="64359-108">If using Seamless Single Sign-on in your application, see [customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span></span>

<span data-ttu-id="64359-109">**Зіставлення атрибутів тверджень**</span><span class="sxs-lookup"><span data-stu-id="64359-109">**Claims Attribute Mapping**</span></span>

1. <span data-ttu-id="64359-110">Щоб настроїти політику зіставлення тверджень за допомогою PowerShell, перегляньте статтю [настроїти претензії, що випускаються в маркерів для певної програми в клієнті (ознайомлювальну версію)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span><span class="sxs-lookup"><span data-stu-id="64359-110">To configure claims mapping policy using PowerShell, see [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
2. <span data-ttu-id="64359-111">Атрибути розширення схеми каталогів дають змогу зберігати додаткові дані в Лазурому Active Directory на об'єктах користувача та інших об'єктах каталогу, як-от групи, відомості про клієнта, керівники служб.</span><span class="sxs-lookup"><span data-stu-id="64359-111">Directory schema extension attributes provide a way to store additional data in Azure Active Directory on user objects and other directory objects such as groups, tenant details, service principals.</span></span> <span data-ttu-id="64359-112">Для застосування позовів до програм можна використовувати лише атрибути розширення для об'єктів користувача.</span><span class="sxs-lookup"><span data-stu-id="64359-112">Only extension attributes on user objects can be used for emitting claims to applications.</span></span> <span data-ttu-id="64359-113">[За допомогою атрибутів розширення схем каталогів у позовах](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) розповідається про те, як використовувати атрибути розширення схем каталогів для надсилання даних користувача до програм у позовах маркерів.</span><span class="sxs-lookup"><span data-stu-id="64359-113">[Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) describes how to use directory schema extension attributes for sending user data to applications in token claims.</span></span>

<span data-ttu-id="64359-114">Докладні відомості про твердження маркерів наведено в статті:</span><span class="sxs-lookup"><span data-stu-id="64359-114">For more information on token claims, see:</span></span>

- [<span data-ttu-id="64359-115">Скарги в маркери доступу</span><span class="sxs-lookup"><span data-stu-id="64359-115">Claims in access tokens</span></span>](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [<span data-ttu-id="64359-116">Скарги в id_token</span><span class="sxs-lookup"><span data-stu-id="64359-116">Claims in an id_token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- <span data-ttu-id="64359-117">[Твердження](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) про те, що ви можете розраховувати на маркери ідентифікаторів і маркери доступу, видані за допомогою AZURE AD B2C</span><span class="sxs-lookup"><span data-stu-id="64359-117">[Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) that you can expect in ID tokens and access tokens issued by Azure AD B2C</span></span>
- [<span data-ttu-id="64359-118">Довідник із маркерів "САМЛ"</span><span class="sxs-lookup"><span data-stu-id="64359-118">SAML token claims reference</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
