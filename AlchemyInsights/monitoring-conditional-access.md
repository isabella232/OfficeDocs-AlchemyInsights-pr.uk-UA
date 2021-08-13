---
title: Моніторинг умовного доступу
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: 80e8cc72db8ae32445d48e5c8a411d5ccd538626653260b3dbd28a247561e888
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975122"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Моніторинг умовного доступу для Exchange

Користувачі, для яких установлено умовний доступ, отримають сповіщення електронною поштою, якщо вони не відповідають вимогам до доступу вашої організації. Щоб вирішити цю проблему, радимо один або кілька з наведених нижче рішень.

- Якщо припустити, що пристрій увімкнулись, порадьте користувачу перейти в програму Company Portal та переконатися, що він відображається в Company Portal. Якщо це не так, користувач має затвердити пристрій.
- На порталі Azure виберіть Intune > Device compliance (Intune). У розділі Монітор клацніть Відповідність пристроїв. Перегляньте звіт про відповідність пристрою, щоб переконатися, що пристрій позначено як відповідний.
- На порталі Azure виберіть Intune > Device compliance (Intune). У розділі Manage (Керування) виберіть Policies (Політики). У списку політик відповідності переконайтеся, що пристрою користувача призначено профіль. Якщо профіль не призначено, Intune не підтвердить відповідність пристрою вимогам.
- Змініть призначення умовного доступу користувача.

1. На порталі Azure виберіть Політики  >  **умовного**  >  **доступу** Intune .
2. Виберіть політику зі списку.
3. Виберіть елемент Користувачі та групи.
4. Щоб цільова політика користувача, додайте їх до списку Include (Включити). Щоб не подавати користувача з політики, додайте його до списку Exclude (Виключити).

Корисні посилання:

[Огляд відповідності пристрою](https://docs.microsoft.com/intune/device-compliance-get-started)

[Виправлення неполадок, пов'язаних із центром спільного редагування](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Виправлення неполадок із політикою](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Моніторинг відповідності пристрою Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

Примітка. Ці дії корисні лише для виправлення неполадок, Azure Active Directory з умовним доступом. Ви також можете перемісити пристрій, який блокує доступ до електронної пошти, Exchange політику. Докладні відомості Exchange про керування пристроєм можна знайти [тут]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
