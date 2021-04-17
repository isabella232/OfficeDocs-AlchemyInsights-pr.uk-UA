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
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821432"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Вирішення проблем із доставкою електронної пошти для коду помилки 5.7.23

Перевірте запис DNS SPF для свого домену в загальнодоступному перевіркі записів SPF або DNS в Інтернеті.

Переконайтеся, що корпорація Майкрософт не визначила вихідне повідомлення як спам і направила його через пул доставки з високим [ризиком.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) Повідомлення в пулі доставки з високим ризиком не проходять перевірки SPF, тому не прийматимуться цільовою організацією електронної пошти.

Якщо проблема не зникне, можливо, знадобиться звернутися до адміністратора поштового хоста, до якого ви намагаєтеся надіслати електронний лист. Занотувати докладну зовнішню помилку, доступну в звіті про незабаром. Можливо, службі підтримки Microsoft не вдасться допомогти.
