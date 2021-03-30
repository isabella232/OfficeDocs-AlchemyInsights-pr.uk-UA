---
title: Програма автентифікації
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405685"
---
# <a name="authentication-app"></a><span data-ttu-id="5cea2-102">Програма автентифікації</span><span class="sxs-lookup"><span data-stu-id="5cea2-102">Authentication app</span></span>

<span data-ttu-id="5cea2-103">Якщо ви глобальний адміністратор, ви можете швидко дізнатися, що сталося, або діагностувати проблеми, пов'язані з входом, за допомогою засобу діагностики [входу.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="5cea2-103">If you are a Global Admin, you can quickly find out what happened or diagnose problems related to user-sign in by using the [Sign-in Diagnostics](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>

1. <span data-ttu-id="5cea2-104">Запустіть діагностику, натиснувши кнопку["Запустити діагностичну".](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="5cea2-104">Start the diagnostics by clicking "[Launch Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" button.</span></span> 
1. <span data-ttu-id="5cea2-105">Знайдіть подію, яку потрібно проаналізувати, ввівши дані про користувача, програму, час входу, ідентифікатор запиту або ідентифікатор кореляції.</span><span class="sxs-lookup"><span data-stu-id="5cea2-105">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="5cea2-106">Перегляньте результати діагностики з відомостями про те, що відбулося, і дії, які можна внести, щоб внести зміни, якщо потрібно внести зміни.</span><span class="sxs-lookup"><span data-stu-id="5cea2-106">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="5cea2-107">**Перегляньте відповідний сценарій.**</span><span class="sxs-lookup"><span data-stu-id="5cea2-107">**Check the scenario that is applicable:**</span></span>

1. <span data-ttu-id="5cea2-108">Якщо користувач не отримує push-сповіщення в програмі Microsoft Authenticator, переконайтеся, що їх не відображаються під заблокованими користувачами багатофаквартирної автентифікації, як описано в статті Блокування та розблокування [користувачів.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="5cea2-108">If a user is not getting a push notification in the Microsoft Authenticator app, verify they are not shown under the MFA blocked users as described in [Block and unblock users](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
1. <span data-ttu-id="5cea2-109">Якщо користувач не блокується для багатофазної автентифікації, але не отримує push-сповіщення, він може відкрити програму Microsoft Authenticator, яка тягне запити на затвердження, що очікують.</span><span class="sxs-lookup"><span data-stu-id="5cea2-109">If the user is not blocked for MFA but does not receive a push notification, they can open the Microsoft Authenticator app, which will pull the pending approval requests.</span></span>
1. <span data-ttu-id="5cea2-110">Як альтернативний спосіб входу користувач може також натиснути кнопку Увійти та вибрати код перевірки з мобільної програми.</span><span class="sxs-lookup"><span data-stu-id="5cea2-110">As an alternative sign-in method, the user can also click on Sign in another way and choose use a verification code from my mobile app.</span></span>
1. <span data-ttu-id="5cea2-111">Microsoft Authenticator App – це єдиний доступний спосіб для багатьох користувачів.</span><span class="sxs-lookup"><span data-stu-id="5cea2-111">The Microsoft Authenticator App is the only available method for many users.</span></span> <span data-ttu-id="5cea2-112">[Докладні відомості про стандартні параметри безпеки](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), див. в статті Запитання й відповіді про програму [Authenticator,](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) які часто ставляться та як вирішити їх.</span><span class="sxs-lookup"><span data-stu-id="5cea2-112">[Learn more about security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), check [Authenticator App FAQ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for commonly asked questions and how to resolve them.</span></span>
 
<span data-ttu-id="5cea2-113">**Рекомендовані відео**</span><span class="sxs-lookup"><span data-stu-id="5cea2-113">**Recommended Videos**</span></span>

<span data-ttu-id="5cea2-114">[Як налаштувати програму Authenticator на новому телефоні (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="5cea2-114">[How to set up Authenticator App on a new phone (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span></span>
