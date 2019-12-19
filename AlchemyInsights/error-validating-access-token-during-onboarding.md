---
title: Сталася помилка під час перевірки маркер доступу до помилки робочого стола аналітика на посадку
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741304"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>"Помилка перевірки маркер доступу" помилка під час робочого стола Analytics, публікування

Ця помилка зазвичай спостерігається після завершення терміну дії маркера автентифікації. Зазвичай оновлення сторінки оновлюється маркером. Проте ця проблема може зберігатися, якщо є будь-які політики умовного доступу, застосовані до облікового запису, що використовується для настільних Analytics. Ви можете переглянути Azure AD входу в журналах Azure портал, щоб дізнатися, чи є будь-які неполадки входу для облікового запису, який використовується для публікування на робочому столі Analytics.

Щоб отримати додаткові відомості про умовний доступ, відвідайте [план розгортання умовного доступу](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).