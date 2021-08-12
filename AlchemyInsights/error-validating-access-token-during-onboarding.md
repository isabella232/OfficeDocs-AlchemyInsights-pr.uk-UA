---
title: Під час аналітики desktop Analytics під час перевірення маркера доступу сталася помилка
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 1d6b840e731eaff537d8f74f9ce0af29af13bd390e701fb2835e8718b4521158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946636"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Під час підключення до Desktop Analytics сталася помилка під час перевірки маркера доступу

Зазвичай ця помилка виникає після завершення терміну дії маркера автентифікації. Зазвичай після оновлення сторінки оновлюється маркер. Однак ця проблема може виникати, якщо до облікового запису застосовуються будь-які політики умовного доступу, застосовані до борту Desktop Analytics. Ви можете переглянути журнали входу в Azure AD на порталі Azure, щоб дізнатися, чи не вдається ввійти в обліковий запис, який використовується для підключення до Desktop Analytics.

Докладні відомості про умовний доступ див. в [цьому документі.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)