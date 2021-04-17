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
ms.openlocfilehash: 06ded694893c020f862864215700853b19d35f08
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820199"
---
# <a name="blocking-legacy-authentication"></a>Блокування застарілої автентифікації

Застаріла автентифікація – це термін, який посилається на запит автентифікації, який здійснюються:

- Старі клієнти Office, які не використовують сучасну автентифікацію (наприклад, клієнт Office 2010).

- Клієнт, який використовує застарілі протоколи пошти, як-от IMAP або SMTP/POP3.

Докладні відомості про блокування застарілої автентифікації та ввімкнення сучасної автентифікації див. в розділі Блокування [застарілої автентифікації.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)

Стандартні параметри безпеки в Azure Active Directory (Azure AD) спрощують захист і захист організації. Стандартні параметри безпеки містять попередньо настроєні параметри безпеки для поширених атак.
Докладні відомості про стандартні параметри безпеки див. в цьому [документі.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) 

**Примітка.** Якщо ваш клієнта створено 22 жовтня 2019 р. або після неї, імовірно, ви за замовчуванням почнете нову поведінку, захищену за замовчуванням, і в клієнта вже активовано стандартні параметри безпеки.  Щоб захистити всіх користувачів, параметри безпеки буде розгорнуто для всіх нових клієнтів.
