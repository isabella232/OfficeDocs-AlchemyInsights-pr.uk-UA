---
title: Використання профілів електронної пошти з InTune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555757"
---
# <a name="using-email-profiles-with-intune"></a>Використання профілів електронної пошти з InTune

InTune можна використовувати для створення та розгортання профілів електронної пошти для власного (вбудованого) поштового клієнта на кількох платформах пристрою.

Для отримання відомостей про деякі обмеження, пов'язані з профілями електронної пошти, зокрема про те, як обробляються наявні профілі та як видаляти профілі [електронної пошти, див.](https://docs.microsoft.com/intune/email-settings-configure)

Щоб отримати додаткові відомості про створення профілів електронної пошти для кожної платформи пристрою, див.:

[Налаштування пристрою Android для налаштування електронної пошти, аутентифікації та синхронізації в InTune](https://docs.microsoft.com/intune/email-settings-android)  
[Додавання параметрів електронної пошти для пристроїв iOS і Ipадос у Microsoft InTune](https://docs.microsoft.com/intune/email-settings-ios)  
[Параметри профілю електронної пошти в Microsoft InTune для пристроїв під керуванням Windows Phone 8,1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Параметри профілю електронної пошти для пристроїв під керуванням Windows 10 у Microsoft InTune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Поширені проблеми синхронізації**

**НОКС на Android профіль електронної пошти забороняє користувачам контакти, календар і завдання, від синхронізації до користувача пристроїв.**

НОКС на андроїд НОКС профіль електронної пошти пропонує адміністратору можливість вирішити, які типи вмісту синхронізуються з пристроєм, встановивши кожен включений.

Якщо параметр для будь-якого типу вмісту налаштовано **не настроєно** (за промовчанням), цей тип вмісту не синхронізуватиметься автоматично. Користувач може ввімкнути тип вмісту, який вони хочуть безпосередньо на пристрої вручну, але цю конфігурацію буде перезаписано параметром політики InTune, а для цього типу вмісту припиняється синхронізація.

