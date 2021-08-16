---
title: Проблеми з умовним доступом
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
ms.openlocfilehash: 85cbd89e461f36a51eed816619fd132ea60dfdb0014eb850c7ec3f38d41e1ca2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069985"
---
# <a name="conditional-access-issues"></a>Проблеми з умовним доступом

**Вирішення проблем із діагностичним входом**

Можна швидко дізнатися, що сталося або діагностувати проблеми, пов'язані із входом, за допомогою засобу [діагностики входу.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Запустіть засіб діагностики входу.
1. Знайдіть подію, яку потрібно проаналізувати, ввівши дані про користувача, програму, час входу, ідентифікатор запиту або ідентифікатор кореляції.
1. Перегляньте результати діагностики з відомостями про те, що відбулося та які дії можна внести, щоб внести зміни (за потреби).

**Кроки з усунення несправностей із входом** 

1. Перейдіть на сторінку входу в Azure AD.
1. Фільтрувати вхід за користувачем, діапазоном часу, програмою, станом, клієнтською програмою тощо.
1. Виберіть подію для входу та перегляньте вкладку Умовний доступ, щоб дізнатися, які політики перевірено.
1. Клацніть рядок політики, щоб переглянути відомості про політику та з'ясувати, чому вона застосована.

**Засоби для усунення несправностей із політикою умовного доступу**

- Режим лише для звітів дає змогу оцінювати політику, не впливаючи на користувачів.
- Інструмент "What-if" дає змогу зімітувати події входу та побачити, які політики застосовуються.
- Аналітика і книга звітування відображає вплив кожної політики в реальному часі.

**Базові політики захисту**

Політики базового захисту вилучено. Вони більше не застосовуються, і їх незабаром буде видалено з порталу Azure. Ми радимо ввімкнути [параметри безпеки за замовчуванням](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).

Докладні відомості про умовний доступ див. в:

[Практичні поради з умовного доступу в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Умови умовного доступу](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Елементи керування в умовного доступу](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Locations in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
