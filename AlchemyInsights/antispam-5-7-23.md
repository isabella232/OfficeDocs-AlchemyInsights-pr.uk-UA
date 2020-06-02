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
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506464"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Вирішення проблем із доставкою електронної пошти для коду помилки 5.7.23

Перевірте SPF запис DNS для домену на загальнодоступних SPF або DNS-запис перевірки в Інтернеті.

Переконайтеся, що вихідне повідомлення не було ідентифіковано як спам від корпорації Майкрософт і спрямовується через [пул доставки з високим ризиком](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). Повідомлення в пул з високим ризиком не пройде SPF перевірки, і тому не буде прийнята організація електронної пошти призначення.

Якщо проблема повторюється, можливо, знадобиться звернутися до адміністратора поштового хоста, до якого ви намагаєтеся надіслати електронний лист. Запишіть докладну зовнішню помилку, доступну в повідомленні відмов. Служба підтримки Microsoft може не бути в змозі допомогти далі.
