---
title: Антиспам – 5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717346"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Вирішення проблем із доставкою електронної пошти для коду помилки 5.7.23

Переконайтеся, що запис DNS SPF для вашого домену перебуває в загальнодоступній версії SPF або записі DNS в Інтернеті.

Переконайтеся, що вихідне повідомлення не було визначено як спам від корпорації Майкрософт і маршрутизується через [високий пул доставки ризиків](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). Повідомлення в пулі з високим ризиком не передаватимуться на перевірку SPF, і тому її не буде прийнято організацією електронної пошти призначення.

Якщо проблему не вирішено, можливо, знадобиться звернутися до адміністратора поштового хоста, до якого ви намагаєтеся надіслати повідомлення електронної пошти. Зверніть увагу на додаткову зовнішню помилку, доступну в повідомленні відмов. Служба підтримки Microsoft може не допомагати надалі.
