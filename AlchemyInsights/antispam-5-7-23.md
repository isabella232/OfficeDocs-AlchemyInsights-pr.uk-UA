---
title: Antispam - 5.7.23
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
- "3156"
- "9001196"
ms.openlocfilehash: cb9073306c65b09813290d6c8470d14395d2836fa3048f8ce0ecb8b06e71a010
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932190"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Вирішення проблем із доставкою електронної пошти для коду помилки 5.7.23

Перевірте запис DNS SPF для свого домену в загальнодоступному перевіркі записів SPF або DNS в Інтернеті.

Переконайтеся, що корпорація Майкрософт не визначила вихідне повідомлення як спам і направила його через пул доставки з високим [ризиком.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) Повідомлення в пулі доставки з високим ризиком не проходять перевірки SPF, тому не прийматимуться цільовою організацією електронної пошти.

Якщо проблема не зникне, можливо, знадобиться звернутися до адміністратора поштового хоста, до якого ви намагаєтеся надіслати електронний лист. Занотувати докладну зовнішню помилку, доступну в звіті про незабаром. Можливо, службі підтримки Microsoft не вдасться допомогти.
