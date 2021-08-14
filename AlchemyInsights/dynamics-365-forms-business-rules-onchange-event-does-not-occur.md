---
title: Бізнес-правила для форм Dynamics 365 Forms – бізнес-правило, яке не потрібно фільтрувати для форми
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 8425918950e1ef6c44f2866e6fa8987fe165536ae21e08ea6a1da880f761d512
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53947320"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Подія OnChange не відбувається, якщо поле змінюється програмно

Подія *OnChange* не відбувається, якщо поле змінюється програмно за допомогою *атрибута.* [метод setValue.](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) Якщо потрібно, щоб обробники подій для події *OnChange* запускалось, коли встановлено значення, у коді потрібно використовувати *атрибут formContext.data.entity* [fireOnchange.](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange)

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
