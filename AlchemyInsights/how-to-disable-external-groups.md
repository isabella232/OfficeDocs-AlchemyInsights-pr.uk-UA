---
title: Як відключити зовнішні групи
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 2159feb4aa3999072de57d76790a2959c7355976
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720789"
---
# <a name="how-to-disable-external-groups"></a>Як відключити зовнішні групи

За зовнішнім повідомленнями Yammer застосовуються правила транспортування Exchange (ETRs), набір проактивних елементів керування, які забороняють спільний доступ до інформації про компанію. Для того, щоб заборонити користувачам створювати зовнішні групи, потрібно настроїти правило транспортування Exchange (ETR), а потім настроїти Yammer для використання правила транспортування Exchange для блокування зовнішніх повідомлень.
  
Після того, як ви створили правило в Exchange Online центру адміністрування, виконайте такі дії, щоб установити ETR для застосування в Yammer:
  
- Увійдіть до Yammer як перевірений адміністратор, а в **центрі адміністрування Yammer**перейдіть до розділу ** \> вміст і параметри безпеки.**

- У розділі **зовнішні повідомлення**виберіть елемент **застосувати правила транспортування Exchange Online (etrs) у Yammer.**

- Виберіть **зберегти**.

Для отримання додаткових відомостей див. [вимкнення зовнішніх повідомлень у мережі Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  