---
title: Настроювання й розширення терміну дії маркера
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917200"
---
# <a name="configure-and-extend-token-lifetimes"></a><span data-ttu-id="eebc3-102">Настроювання й розширення терміну дії маркера</span><span class="sxs-lookup"><span data-stu-id="eebc3-102">Configure and extend token lifetimes</span></span>

<span data-ttu-id="eebc3-103">Ви можете вказати термін дії доступу, САМЛ або ІДЕНТИФІКАТОРА, виданий платформою Microsoft Identity.</span><span class="sxs-lookup"><span data-stu-id="eebc3-103">You can specify the lifetime of an access, SAML, or ID token issued by Microsoft identity platform.</span></span> <span data-ttu-id="eebc3-104">Ви можете встановити термін служби маркерів для всіх програм у вашій організації, для багатоклієнтської програми (мульти-організація) або для певної основної служби в організації.</span><span class="sxs-lookup"><span data-stu-id="eebc3-104">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> <span data-ttu-id="eebc3-105">Щоб отримати докладні відомості, ознайомтеся з [настроюваним терміном існування маркера](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="eebc3-105">For more info, read [configurable token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="eebc3-106">Наприклад, ознайомтеся [з прикладами того, як настроїти тривалість роботи маркера](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="eebc3-106">For examples, read [examples of how to configure token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span></span>

<span data-ttu-id="eebc3-107">Щоб дізнатися, як настроїти тривалість життя та сумісність маркера в Лазурові Active Directory B2C (Azure AD B2C), перегляньте статтю [настроїти маркери в полі Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span><span class="sxs-lookup"><span data-stu-id="eebc3-107">To learn how to configure the lifetime and compatibility of a token in Azure Active Directory B2C (Azure AD B2C), see [Configure tokens in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span></span>

<span data-ttu-id="eebc3-108">У статті [Настроювання поведінки сеансу в Лазур Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) описує методи єдиного входу (SSO), які використовуються в ЛАЗУРОВІ B2C, і дає змогу вибрати найбільш підходящий метод єдиного входу під час настроювання політики.</span><span class="sxs-lookup"><span data-stu-id="eebc3-108">The article [Configure session behavior in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) describes the single sign-on (SSO) methods used in Azure AD B2C and helps you choose the most appropriate SSO method when configuring your policy.</span></span>

<span data-ttu-id="eebc3-109">**Як довго тривають маркери? Як довго вони діють?**</span><span class="sxs-lookup"><span data-stu-id="eebc3-109">**How long do tokens last? How long are they valid for?**</span></span>

<span data-ttu-id="eebc3-110">Термін дії маркера – 1 година, а тривалість сеансу – 24 години.</span><span class="sxs-lookup"><span data-stu-id="eebc3-110">Token lifetimes are 1 hour and the session lifetime is 24 hours.</span></span> <span data-ttu-id="eebc3-111">Це означає, що якщо не вдалося виконати запит протягом 24 годин, перш ніж запитувати новий маркер, потрібно знову ввійти знову.</span><span class="sxs-lookup"><span data-stu-id="eebc3-111">This means that if no requests have been made in 24 hours, you will need to log in again before requesting a new token.</span></span>

> [!NOTE]
> <span data-ttu-id="eebc3-112">Після 30 травня 2020, жоден новий клієнт не зможе використовувати настроювані правила Lifetime для настроювання сеансу та оновлення маркерів.</span><span class="sxs-lookup"><span data-stu-id="eebc3-112">After May 30, 2020, no new tenant will be able to use Configurable Token Lifetime policy to configure session and refresh tokens.</span></span> <span data-ttu-id="eebc3-113">Після цього відбудеться протягом кількох місяців після цього, що означає, що ми припиняємо на честь наявного сеансу та оновити маркери.</span><span class="sxs-lookup"><span data-stu-id="eebc3-113">The deprecation will happen within several months after that, which means that we will stop honoring existing session and refresh tokens polices.</span></span> <span data-ttu-id="eebc3-114">Ви все ще можете налаштувати час існування маркера доступу після закінчення.</span><span class="sxs-lookup"><span data-stu-id="eebc3-114">You can still configure access token lifetimes after the deprecation.</span></span>






