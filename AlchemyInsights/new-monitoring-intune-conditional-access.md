---
title: Моніторинг умовного доступу Intune
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: 2c3a382671ac95ecbaec1b374bd8c474cf9690a2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327578"
---
# <a name="monitor-intune-conditional-access"></a>Моніторинг умовного доступу Intune

Користувачі, для яких установлено умовний доступ, отримають сповіщення електронною поштою, якщо вони не відповідають вимогам до доступу вашої організації. Щоб вирішити цю проблему, радимо один або кілька з наведених нижче рішень.

1. Якщо припустити, що пристрій увімкнулись, порадьте користувачу перейти в програму Company Portal та переконатися, що він відображається в Company Portal. Якщо це не так, користувач має затвердити пристрій.
1. На порталі Azure виберіть Intune Device compliance **(Відповідність пристроїв Intune).**  >   
1. Щоб переглянути звіт про відповідність пристрою вимогам, щоб переконатися, що пристрій позначено як відповідний, у розділі Монітор **клацніть** **Відповідність пристроїв**.
1. На порталі Azure виберіть Intune Device compliance **(Відповідність пристроїв Intune).**  >   У **розділі Manage (Керування)** клацніть **Policies (Політики).** У списку політик відповідності переконайтеся, що пристрою користувача призначено профіль. Якщо профіль не призначено, Intune не підтвердить відповідність пристрою вимогам.
1. Змініть призначення умовного доступу користувача.
1. На порталі Azure перейдіть до пункту Політики умовного доступу **Intune**, виберіть політику зі списку  >    >  та клацніть **Користувачі та групи**.
1. Щоб цільову політику користувача, додайте їх до списку **Include (Включити).** Щоб не подавати користувача з політики, додайте його до списку **Exclude (Виключити)**.

**Корисні посилання:**

- [Огляд відповідності пристрою](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Виправлення неполадок, пов'язаних із центром спільного редагування](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Виправлення неполадок із політикою](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Моніторинг відповідності пристрою Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

**Примітка.** Ці дії стануть у нагоді під час виправлення неполадок Azure Active Directory умовного доступу. Крім того, ви можете перемісити пристрій, який блокує доступ до електронної пошти, Exchange політику. Докладні відомості Exchange керування пристроями можна знайти [**тут.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))
