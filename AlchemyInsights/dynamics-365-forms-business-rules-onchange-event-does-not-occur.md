---
title: Dynamics 365 форм бізнес-правила-бізнес-правила не стрілянину для форми
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 3cdd2175083e864b3bffc57a70bb6c6220843fad
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 11/15/2019
ms.locfileid: "37769360"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>OnChange події не виникає, якщо поле змінено програмним способом

Подія *OnChange* не виникає, якщо поле змінено програмно за допомогою *атрибута.* метод [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . Якщо ви бажаєте, щоб обробники подій *OnChange* події запусквиконуватися після встановлення значення, необхідно використовувати метод *formcontext. Data. сутність* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) методу у коді.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
