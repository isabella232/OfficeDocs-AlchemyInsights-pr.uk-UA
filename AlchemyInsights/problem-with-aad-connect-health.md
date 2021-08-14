---
title: Проблема з AAD Підключення справності
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: 82cfcc6132549b52278b174fce3173f5566268864a207882a4dd639cb8024ee3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923773"
---
# <a name="problem-with-aad-connect-health"></a>Проблема з AAD Підключення справності

- Переконайтеся, що ви маєте право виконувати операцію. За замовчуванням глобальні адміністратори мають доступ. Крім того, ви можете [використовувати](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) керування доступом на основі ролей, щоб делегувати дозвіл на реєстрацію вповноваженому учаснику.
- Переконайтеся, що обов'язкові кінцеві точки ввімкнуто й не заблоковано через брандмауер. Докладні відомості див. у [вимогах](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Реєстрація може не вдатися через те, що вихідне спілкування підлягає перевіркі SSL через мережевий рівень.
- Переконайтеся, що ви підтвердили параметри сповіщень для Azure AD Підключення Health. Перевірте настройку. Цей [посібник](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) допоможе вам зрозуміти, як налаштувати параметри сповіщень для Azure AD Підключення сповіщення про справність.
- Докладні відомості про звіт про синхронізацію AAD Підключення справність і про те, як його завантажити, див. в статті Звіт про синхронізацію [на рівні об'єктів.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Щоб виправити неполадки зі сповіщеннями AAD Підключення справності, дотримуйтеся вказівок із виправлення неполадок для оповіщень про оновлення даних [AAD Підключення](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) справності та поширених запитань про поширені запитання про інсталяцію [AAD Підключення справності.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)
