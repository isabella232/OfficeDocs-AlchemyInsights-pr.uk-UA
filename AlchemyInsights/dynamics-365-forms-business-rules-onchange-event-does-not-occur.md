---
title: Динаміка 365 форми бізнес-правил – правило для бізнесу не стріляв для форми
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
ms.openlocfilehash: 7422b67973f93ce10c1639209cc50206a1016c10
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711512"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Подія OnChange не виникає, якщо поле змінено програмно

Подія *Onchange* не виникає, якщо поле змінено програмно за допомогою *атрибута.* метод [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . Якщо ви хочете, щоб обробники подій для події *Onchange* запускалася після того, як ви встановили значення, яке потрібно використовувати для параметра *formcontext. Data. атрибут* [fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) в коді.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
