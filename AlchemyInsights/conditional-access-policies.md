---
title: Політики умовного доступу
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002357"
- "4583"
ms.openlocfilehash: 8ce41d007988f2a45f1ded385ae50ac3def97c1b
ms.sourcegitcommit: 9923ce61344e22c4490549b12f65fa2896490b1f
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/01/2020
ms.locfileid: "43100641"
---
# <a name="conditional-access-policies"></a>Політики умовного доступу

Умовний доступ – це можливість Azure AD застосовувати елементи керування під час доступу до програм у вашому середовищі, відповідно до конкретних умов, а також керувати ними з центрального розташування.

Докладні відомості див. у статті [Умовний доступ Azure AD](https://docs.microsoft.com/azure/active-directory/conditional-access/).  

**Примітка**. Якщо ваш клієнт створено після 21 жовтня 2019 р. і ви неочікувано отримуєте запит на проведення БФА, ймовірно, у вашому клієнті увімкнено [стандартні параметри безпеки](http://aka.ms/securitydefaults).

**Щоб керувати стандартними параметрами безпеки, зробіть ось що.**

1. Увійдіть у [Центр адміністрування](https://go.microsoft.com/fwlink/p/?linkid=834822) за допомогою облікових даних глобального адміністратора.

2. Перейдіть у розділ [Властивості Azure Active Directory](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).

3. У нижній частині сторінки виберіть **Керування стандартними параметрами безпеки**.

4. Натисніть кнопку **Так**, щоб увімкнути стандартні параметри безпеки, або **Ні**, щоб їх вимкнути.
