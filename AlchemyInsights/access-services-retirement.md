---
title: Викид служб Access
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
ms.openlocfilehash: 32da879de230dc0ed99563ad881ab5b2479b8453933a127961a26d619e108ab9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938716"
---
# <a name="access-services-retirement"></a>Викид служб Access

У березні 2017 року ми оголосили про це в MC97576 і продовжували спілкуватися протягом минулого служби Access Services року. Наступний етап цього процесу – видалення веб-баз даних Access, у яких використовуються SharePoint списки як основне сховище даних.

**Як це вплине на мене?**

Починаючи з червня 2019 р., ми припинимо створювати нові бази даних Access у SharePoint Online і закриємо службу та решту програм до квітня 2020 р.

**Як підготуватися до цієї зміни?**

Радимо створити план переходу для веб-баз даних Access організації. Адміністратори можуть використовувати [сканер SharePoint Access,](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) щоб отримати інвентарний список веб-програм Access, які використовуються на сайтах.

Перенести дані веб-баз даних Access можна кількома способами:

- Імпорт до локальної бази даних Access (. ACCDB) або до Excel файлу.
- Ми також рекомендуємо вивчати Microsoft PowerApps як альтернативну платформу, щоб створювати бізнес-рішення без коду для веб-сторінок і мобільних пристроїв.