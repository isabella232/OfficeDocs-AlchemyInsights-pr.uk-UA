---
title: Політики умовного доступу
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002357"
- "4583"
ms.openlocfilehash: af95627d07d41add54f03c9254562b9be4e05d9b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817301"
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
