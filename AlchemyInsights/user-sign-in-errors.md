---
title: Помилки входу користувачів
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7790"
- "9004355"
ms.openlocfilehash: 05bd31cb4afecf1342e040eecd9e58cd38bd8d49
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901249"
---
# <a name="user-sign-in-errors"></a><span data-ttu-id="327aa-102">Помилки входу користувачів</span><span class="sxs-lookup"><span data-stu-id="327aa-102">User sign-in errors</span></span>

<span data-ttu-id="327aa-103">**Вирішення проблем із діагностичною програмою для входу**</span><span class="sxs-lookup"><span data-stu-id="327aa-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="327aa-104">Щоб виявити причину або діагностику проблем, пов'язаних із входом користувача, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="327aa-104">To detect the cause or diagnose problems related to user sign-in, perform the following steps:</span></span>

1. <span data-ttu-id="327aa-105">Запустіть [діагностику для входу](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span><span class="sxs-lookup"><span data-stu-id="327aa-105">Launch the [Sign-in Diagnostic](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
2. <span data-ttu-id="327aa-106">Знайти подію для аналізу, ввівши відомості про користувача, програму, час входу, ідентифікатор запиту або ідентифікатор кореляції.</span><span class="sxs-lookup"><span data-stu-id="327aa-106">Find the event to analyze by entering the details you have about the user, application, time of sign in, request Id, or correlation Id.</span></span>
3. <span data-ttu-id="327aa-107">Перегляньте результати діагностики, що містить відомості про те, що сталося, і які дії ви можете внести зміни, якщо необхідні зміни.</span><span class="sxs-lookup"><span data-stu-id="327aa-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="327aa-108">**Шукаєте відомості про коди помилок AADSTS, які повертаються в службі маркерів безпеки "Лазурний" (STS)?**</span><span class="sxs-lookup"><span data-stu-id="327aa-108">**Looking for information about the AADSTS error codes that are returned from the Azure Active Directory (Azure AD) security token service (STS)?**</span></span> <span data-ttu-id="327aa-109">Прочитайте [цю статтю](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) , щоб ознайомитися з описами про помилки, виправленнями та деякими запропонованими обхідні шляхи.</span><span class="sxs-lookup"><span data-stu-id="327aa-109">Read [this article](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) to find AADSTS error descriptions, fixes, and some suggested workarounds</span></span>