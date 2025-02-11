---
title: EndPoint Manager – базові плани безпеки
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
- "10064"
- "9003771"
ms.openlocfilehash: 4c8e03a817751ba7dc1710aed5a3e19c6e79db33
ms.sourcegitcommit: ae556b6b26974392ca68a68426a2b40967ae0071
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/07/2021
ms.locfileid: "58923575"
---
# <a name="endpoint-manager---security-baselines"></a>EndPoint Manager – базові плани безпеки

Базові плани безпеки – це попередньо налаштовані групи параметрів Windows, які допомагають застосувати параметри безпеки, рекомендовані відповідними групами безпеки. Ці базові плани можна настроїти так, щоб вони постачали лише бажані параметри та значення. Докладні відомості про базові плани безпеки див. в статті [Використання базових планів безпеки для настроювання пристроїв із Windows 10 в Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).

Наразі є базові плани для цих продуктів:

- Параметри безпеки MDM у Windows
- Безпека Microsoft Defender для кінцевих точок
- Microsoft Edge

Кожен із базових планів періодично оновлюється та випускається в інкрементних версіях. Кожна версія додає та видаляє параметри з попередньої версії, щоб забезпечити відповідність базового плану поточним рекомендаціям. Консоль безпеки базового плану для кінцевих точок дає змогу порівняти різні версії, показуючи зміни з версії до версії.

Докладні відомості про те, як ефективніше змінити версію застосованого базового плану, див. в статті [Налаштування профілів базового плану безпеки в Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).

Розгорнувши базовий план безпеки, можна відстежувати стан розгортання та переглядати параметри для кожного пристрою.

Оскільки базові плани безпеки містять багато параметрів, важливо перевірити зміни в конфігурації та виконати перевірку, щоб переконатися, що всі параметри підходять для ваших пристроїв і бізнес-потреб.

**Примітка:** Дані звітування для базових планів можуть з'явитися протягом 24 годин від початкового розгортання для пристрою та до 6 годин для подальших оновлень. 

Найпоширеніша причина незастосованого параметра базового плану полягає в тому, що той самий параметр використовується в іншому профілі. Цей сценарій можна дослідити для певного пристрою, вибравши його у вузлі "Стан пристрою" профілю базового плану безпеки. Докладні відомості див. [Вирішення конфліктів для базових планів безпеки](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).