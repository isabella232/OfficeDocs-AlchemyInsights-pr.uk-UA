---
title: Доступ до послуг виходу на пенсію
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 197366882468ebc87fc26f2fe2733371790d1871
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/25/2019
ms.locfileid: "36747809"
---
# <a name="access-services-retirement"></a>Доступ до послуг виходу на пенсію

Як ми спочатку оголосили в MC97576, в березні 2017, і продовжував спілкуватися за минулий рік служби доступу в даний час вийшли з офісу 365. Наступним етапом у цьому процесі буде видалення веб-баз даних Access, які використовують списки SharePoint як основне сховище даних.

**Як це впливає на мене?**

Починаючи з червня 2019, ми зупиняємо створення нових баз даних Access у SharePoint Online і закрили службу та інші додатки до квітня 2020.

**Що потрібно зробити, щоб підготуватися до цієї зміни?**

Радимо створити план переходу для веб-баз даних Access вашої організації. Адміністратори можуть використовувати [сканер застосунку SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) для отримання інвентаризації програм Access, які використовують сайти.

Існує кілька способів перенести дані веб-баз даних Access:

- Імпорт до бази даних локальних Access (. ACCDB) або до файлу Excel.
- Ми також рекомендуємо вивчати Microsoft PowerApps як альтернативну платформу для створення не-коду бізнес-рішень для веб-і мобільних пристроїв.