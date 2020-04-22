---
title: Доступ до послуг виходу на пенсію
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 977bd5887ef58b328463a9befcd6b47ac55f5a85
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687279"
---
# <a name="access-services-retirement"></a>Доступ до послуг виходу на пенсію

Як ми спочатку оголосили в MC97576, в березні 2017, і продовжував спілкуватися за минулий рік послуги доступу в даний час вийшли на пенсію. Наступним етапом у цьому процесі буде видалення веб-баз даних Access, які використовують списки SharePoint як основне сховище даних.

**Як це впливає на мене?**

Починаючи з червня 2019, ми зупиняємо створення нових баз даних Access у SharePoint Online і закрили службу та інші додатки до квітня 2020.

**Що потрібно зробити, щоб підготуватися до цієї зміни?**

Радимо створити план переходу для веб-баз даних Access вашої організації. Адміністратори можуть використовувати [сканер застосунку SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) для отримання інвентаризації програм Access, які використовують сайти.

Існує кілька способів перенести дані веб-баз даних Access:

- Імпорт до бази даних локальних Access (. ACCDB) або до файлу Excel.
- Ми також рекомендуємо вивчати Microsoft PowerApps як альтернативну платформу для створення не-коду бізнес-рішень для веб-і мобільних пристроїв.