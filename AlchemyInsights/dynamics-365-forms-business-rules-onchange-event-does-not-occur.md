---
title: Dynamics 365 утворює бізнес-правил - бізнес-правила, не стрільби для форми
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 4ade8d2f68b465298e2d6efff3eef4f04f25c3bf
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/16/2019
ms.locfileid: "35749113"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>OnChange подія не виникає, якщо на поле змінити програмним способом

*OnChange* подія не виникає, якщо поле є змінити програмним способом за допомогою у *атрибутом.* [Установити значення](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) метод. Якщо ви хочете обробників подій для *OnChange* подія для запуску установлене значення, слід використовувати у *атрибутом formContext.data.entity.* [fireOnchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) метод у вашому коді.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
