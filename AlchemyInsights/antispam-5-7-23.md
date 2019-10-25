---
title: Антиспам-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682346"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Вирішення проблем із доставкою електронної пошти для коду помилки 5.7.23

Перевірте SPF запис DNS для домену на загальнодоступних SPF або DNS-запис перевірки в Інтернеті.

Переконайтеся, що вихідне повідомлення не було визначено як спам, Office 365 і спрямовується через [високий ризик доставки пула](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages). Повідомлення в пул з високим ризиком не пройде SPF перевірки, і тому не буде прийнята організація електронної пошти призначення.

Якщо проблема повторюється, можливо, знадобиться звернутися до адміністратора поштового хоста, до якого ви намагаєтеся надіслати електронний лист. Запишіть докладну зовнішню помилку, доступну в повідомленні відмов.  Підтримка Office 365 може не бути в змозі допомогти далі.