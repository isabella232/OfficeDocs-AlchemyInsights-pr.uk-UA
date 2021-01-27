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
# <a name="conditional-access-issues"></a>Проблеми з умовною доступом

**Вирішення проблем із діагностичною програмою для входу**

Ви можете швидко дізнатися, що сталося або діагностувати проблеми, пов'язані з входом користувача за допомогою [діагностики входу](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):

1. Запустіть діагностику для входу.
1. Знайти подію для аналізу, ввівши відомості про користувача, програму, час входу, ідентифікатор запиту або ідентифікатор кореляції.
1. Перегляньте результати діагностики, на яких показано відомості про те, що сталося, і які дії ви можете внести зміни (якщо потрібні зміни).

**Дії з виправлення неполадок із входом** 

1. Перейдіть на сторінку входу в Azure AD.
1. Фільтрування за допомогою користувача, часового діапазону, застосунку, стану, програми клієнта тощо.
1. Виберіть подію входу та перейдіть на вкладку умовний доступ, щоб дізнатися, які політики було оцінено.
1. Клацніть рядок політики, щоб переглянути відомості про політику та дізнатися, чому вона застосовується.

**Засоби, які допоможуть усунути політику умовного доступу**

- Режим лише для звіту дає змогу оцінити політику без впливу на користувачів.
- Інструмент "what-IF" дає змогу імітувати події входу та бачити, які політики застосовуватимуться.
- У книзі "звіти та звіти" відображаються результати в реальному часі кожної політики.

**Політики захисту від базового плану**

Політики захисту від базової лінії застаріли. Вони більше не виконуються, і незабаром буде видалено з порталу Azure. Радимо ввімкнути [Параметри безпеки за замовчуванням](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).

Докладні відомості про умовний доступ див.

[Практичні поради з умовного доступу в "Лазурний" Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Умови в умовному доступі](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Елементи керування в умовному доступі](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Розташування в умовному доступі](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
