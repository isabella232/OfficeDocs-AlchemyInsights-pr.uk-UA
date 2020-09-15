---
title: Пенсійні служби Access Services
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698703"
---
# <a name="access-services-retirement"></a>Пенсійні служби Access Services

Як ми спочатку анонсували в MC97576, у березні 2017, і продовжували спілкуватися за минулий рік, служби доступу в минулому році перебувають у відставку. Наступний етап у цьому процесі стане видаленням веб-баз даних Access, які використовують списки SharePoint, як їх основний простір.

**Як це вплине на мене?**

Починаючи з червня 2019, ми припиняємо створення нових баз даних Access у службі SharePoint Online і вимкніть службу та решту програм у квітні 2020.

**Що потрібно зробити, щоб підготуватися до цієї зміни?**

Радимо створити план переходу для веб-баз даних організації Access. Адміністратори можуть використовувати [сканер програми SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) , щоб отримати інвентаризацію програм Access, які використовують сайти.

Перенести дані веб-баз даних Access можна кількома способами:

- Імпорт до локальної бази даних Access (. ACCDB) або файл Excel.
- Ми також рекомендуємо вивчати Microsoft PowerApps як альтернативну платформу для створення без коду бізнес-рішень для веб-і мобільних пристроїв.