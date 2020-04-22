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
ms.openlocfilehash: 569507318b499cdbcf2a1cd75e84046953f62212
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706078"
---
# <a name="conditional-access-policies"></a>Політики умовного доступу

Умовний доступ – це можливість Azure AD застосовувати елементи керування під час доступу до програм у вашому середовищі, відповідно до конкретних умов, а також керувати ними з центрального розташування.

Докладні відомості див. у статті [Умовний доступ Azure AD](https://docs.microsoft.com/azure/active-directory/conditional-access/).  

**Примітка**. Якщо ваш клієнт створено після 21 жовтня 2019 р. і ви неочікувано отримуєте запит на проведення БФА, ймовірно, у вашому клієнті увімкнено [стандартні параметри безпеки](https://aka.ms/securitydefaults).

**Щоб керувати стандартними параметрами безпеки, зробіть ось що.**

1. Увійдіть у [Центр адміністрування](https://go.microsoft.com/fwlink/p/?linkid=834822) за допомогою облікових даних глобального адміністратора.

2. Перейдіть у розділ [Властивості Azure Active Directory](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).

3. У нижній частині сторінки виберіть **Керування стандартними параметрами безпеки**.

4. Натисніть кнопку **Так**, щоб увімкнути стандартні параметри безпеки, або **Ні**, щоб їх вимкнути.
