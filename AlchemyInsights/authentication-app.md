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
ms.openlocfilehash: 1ac3158914455502d2de493dd1320034b1d09573ebb3ffef24c23eb1e816cad0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082963"
---
# <a name="authentication-app"></a>Програма автентифікації

Якщо ви глобальний адміністратор, ви можете швидко дізнатися, що сталося, або діагностувати проблеми, пов'язані з входом, за допомогою засобу діагностики [входу.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Запустіть діагностику, натиснувши кнопку["Запустити діагностичну".](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom) 
1. Знайдіть подію, яку потрібно проаналізувати, ввівши дані про користувача, програму, час входу, ідентифікатор запиту або ідентифікатор кореляції.
1. Перегляньте результати діагностики з відомостями про те, що відбулося, і дії, які можна внести, щоб внести зміни, якщо потрібно внести зміни.

**Перегляньте відповідний сценарій.**

1. Якщо користувач не отримує push-сповіщення в програмі Microsoft Authenticator, переконайтеся, що їх не відображаються під заблокованими користувачами багатофаквартирних програм, як описано в статті Блокування та [розблокування користувачів.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)
1. Якщо користувач не блокується для багатофагів, але не отримує push-сповіщення, він може відкрити програму Microsoft Authenticator, яка шахраї отримають запити на затвердження, що очікують.
1. Як альтернативний спосіб входу користувач може також натиснути кнопку Увійти та вибрати код перевірки з мобільної програми.
1. Програма Microsoft Authenticator доступна лише для багатьох користувачів. [Дізнайтеся більше про стандартні параметри](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)безпеки , перегляньте [запитання Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) запитання й відповіді про програму та способи їх вирішення.
 
**Рекомендовані відео**

[Як настроїти програму Authenticator на новому телефоні (2 хвилини)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).
