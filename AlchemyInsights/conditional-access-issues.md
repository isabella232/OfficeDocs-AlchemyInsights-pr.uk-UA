---
title: Проблеми з умовною доступом
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015006"
---
# <a name="conditional-access-issues"></a><span data-ttu-id="01204-102">Проблеми з умовною доступом</span><span class="sxs-lookup"><span data-stu-id="01204-102">Conditional access issues</span></span>

<span data-ttu-id="01204-103">**Вирішення проблем із діагностичною програмою для входу**</span><span class="sxs-lookup"><span data-stu-id="01204-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="01204-104">Ви можете швидко дізнатися, що сталося або діагностувати проблеми, пов'язані з входом користувача за допомогою [діагностики входу](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span><span class="sxs-lookup"><span data-stu-id="01204-104">You can quickly find out what happened or diagnose problems related to user sign-in by using the [Sign-in Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span></span>

1. <span data-ttu-id="01204-105">Запустіть діагностику для входу.</span><span class="sxs-lookup"><span data-stu-id="01204-105">Launch the Sign-in Diagnostic.</span></span>
1. <span data-ttu-id="01204-106">Знайти подію для аналізу, ввівши відомості про користувача, програму, час входу, ідентифікатор запиту або ідентифікатор кореляції.</span><span class="sxs-lookup"><span data-stu-id="01204-106">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="01204-107">Перегляньте результати діагностики, на яких показано відомості про те, що сталося, і які дії ви можете внести зміни (якщо потрібні зміни).</span><span class="sxs-lookup"><span data-stu-id="01204-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes (if any changes are needed).</span></span>

<span data-ttu-id="01204-108">**Дії з виправлення неполадок із входом**</span><span class="sxs-lookup"><span data-stu-id="01204-108">**Steps to Troubleshoot a Sign-In**</span></span> 

1. <span data-ttu-id="01204-109">Перейдіть на сторінку входу в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="01204-109">Navigate to the Azure AD Sign-in page.</span></span>
1. <span data-ttu-id="01204-110">Фільтрування за допомогою користувача, часового діапазону, застосунку, стану, програми клієнта тощо.</span><span class="sxs-lookup"><span data-stu-id="01204-110">Filter sign-ins by user, time range, application, status, client app, and so on.</span></span>
1. <span data-ttu-id="01204-111">Виберіть подію входу та перейдіть на вкладку умовний доступ, щоб дізнатися, які політики було оцінено.</span><span class="sxs-lookup"><span data-stu-id="01204-111">Select a sign-in event and view the Conditional Access tab to see which policies were evaluated.</span></span>
1. <span data-ttu-id="01204-112">Клацніть рядок політики, щоб переглянути відомості про політику та дізнатися, чому вона застосовується.</span><span class="sxs-lookup"><span data-stu-id="01204-112">Click on the row of a policy to view the policy details and understand why it applied.</span></span>

<span data-ttu-id="01204-113">**Засоби, які допоможуть усунути політику умовного доступу**</span><span class="sxs-lookup"><span data-stu-id="01204-113">**Tools to troubleshoot a Conditional Access policy**</span></span>

- <span data-ttu-id="01204-114">Режим лише для звіту дає змогу оцінити політику без впливу на користувачів.</span><span class="sxs-lookup"><span data-stu-id="01204-114">Report-only mode lets you evaluate a policy without impacting users.</span></span>
- <span data-ttu-id="01204-115">Інструмент "what-IF" дає змогу імітувати події входу та бачити, які політики застосовуватимуться.</span><span class="sxs-lookup"><span data-stu-id="01204-115">What-if tool lets you simulate sign-in events and see which policies apply.</span></span>
- <span data-ttu-id="01204-116">У книзі "звіти та звіти" відображаються результати в реальному часі кожної політики.</span><span class="sxs-lookup"><span data-stu-id="01204-116">Insights and reporting workbook displays real-time impact of each policy.</span></span>

<span data-ttu-id="01204-117">**Політики захисту від базового плану**</span><span class="sxs-lookup"><span data-stu-id="01204-117">**Baseline Protection Policies**</span></span>

<span data-ttu-id="01204-118">Політики захисту від базової лінії застаріли.</span><span class="sxs-lookup"><span data-stu-id="01204-118">Baseline Protection policies have been deprecated.</span></span> <span data-ttu-id="01204-119">Вони більше не виконуються, і незабаром буде видалено з порталу Azure.</span><span class="sxs-lookup"><span data-stu-id="01204-119">They are no longer being enforced and will soon be removed from Azure portal.</span></span> <span data-ttu-id="01204-120">Радимо ввімкнути [Параметри безпеки за замовчуванням](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="01204-120">We recommend enabling [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span>

<span data-ttu-id="01204-121">Докладні відомості про умовний доступ див.</span><span class="sxs-lookup"><span data-stu-id="01204-121">For more information on Conditional Access see:</span></span>

<span data-ttu-id="01204-122">[Практичні поради з умовного доступу в "Лазурний" Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Умови в умовному доступі](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Елементи керування в умовному доступі](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Розташування в умовному доступі](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span><span class="sxs-lookup"><span data-stu-id="01204-122">[Best practices for conditional access in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Controls in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
[Locations in Conditional Access ](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span></span>
