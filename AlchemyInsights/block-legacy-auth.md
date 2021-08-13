---
title: BlockLegacyAuth
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
- "3154"
- "9001194"
ms.openlocfilehash: c2f2a0c3888920a969a6fc70af7ef7bfd8435bdcf975e0f31452b5da85e3a208
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53968902"
---
# <a name="blocking-legacy-authentication"></a>Блокування застарілої автентифікації

Застаріла автентифікація – це термін, який посилається на запит автентифікації, який здійснюються:

- Старі Office, які не використовують сучасну автентифікацію (наприклад, клієнт Office 2010).

- Клієнт, який використовує застарілі протоколи пошти, як-от IMAP або SMTP/POP3.

Докладні відомості про блокування застарілої автентифікації та ввімкнення сучасної автентифікації див. в розділі Блокування [застарілої автентифікації.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)

Стандартні параметри безпеки в Azure Active Directory (Azure AD) спрощують захист і захист організації. Стандартні параметри безпеки містять попередньо настроєні параметри безпеки для поширених атак.
Докладні відомості про стандартні параметри безпеки див. в цьому [документі.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) 

**Примітка.** Якщо ваш клієнта створено 22 жовтня 2019 р. або після неї, імовірно, ви за замовчуванням почнете нову поведінку, захищену за замовчуванням, і в клієнта вже активовано стандартні параметри безпеки.  Щоб захистити всіх користувачів, параметри безпеки буде розгорнуто для всіх нових клієнтів.
