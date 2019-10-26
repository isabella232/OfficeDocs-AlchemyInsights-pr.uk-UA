---
title: Як відключити зовнішні групи
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: b2328ea85d3ff6ec722cc56d8a46395d8438f79c
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/25/2019
ms.locfileid: "36739514"
---
# <a name="how-to-disable-external-groups"></a>Як відключити зовнішні групи

За зовнішнім повідомленнями Yammer застосовуються правила транспортування Exchange (ETRs), набір проактивних елементів керування, які забороняють спільний доступ до інформації про компанію. Для того, щоб заборонити користувачам створювати зовнішні групи, потрібно настроїти правило транспортування Exchange (ETR), а потім настроїти Yammer для використання правила транспортування Exchange для блокування зовнішніх повідомлень.
  
Після того, як ви створили правило в Exchange Online центру адміністрування, виконайте такі дії, щоб установити ETR для застосування в Yammer:
  
- Увійдіть до Yammer як перевірений адміністратор, а в **центрі адміністрування Yammer**перейдіть до розділу ** \> вміст і параметри безпеки.**

- У розділі **зовнішні повідомлення**виберіть елемент **застосувати правила транспортування Exchange Online (etrs) у Yammer.**

- Виберіть **зберегти**.

Для отримання додаткових відомостей див. [вимкнення зовнішніх повідомлень у мережі Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  