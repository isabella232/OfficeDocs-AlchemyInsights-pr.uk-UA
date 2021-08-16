---
title: Вимкнення зовнішніх груп
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 9c513da49dc953b4ae76bb06854e33232ec40e11151f11ade33c3080092aa598
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54015641"
---
# <a name="how-to-disable-external-groups"></a>Вимкнення зовнішніх груп

Yammer обміну повідомленнями із зовнішніми користувачами застосовується Exchange правил транспортування – набір завадних елементів керування, які запобігають обміну корпоративною інформацією. Щоб заборонити користувачам створювати зовнішні групи, потрібно налаштувати правило транспортування Exchange (ETR), а потім настроїти Yammer на використання правила транспортування Exchange для блокування обміну повідомленнями із зовнішніми користувачами.
  
Створиивши правило в Центрі адміністрування Exchange Online, виконайте наведені нижче дії, щоб налаштувати застосування правил ETR у Yammer:
  
- Увійдіть в Yammer як перевірений адміністратор і в **Центрі адміністрування Yammer** перейдіть до пункту C Вміст і безпека **\> Настройки.**

- У **розділі Зовнішні повідомлення** виберіть Примусовий Exchange Online Exchange правила транспортування **(ETRS)** у Yammer.

- Натисніть **кнопку Зберегти.**

Докладні відомості див. [в цій Yammer мережі.](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging)
  