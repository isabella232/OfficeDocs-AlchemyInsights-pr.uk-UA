---
title: Вхід для Windows 10 без використання пароля
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: fbf190d433eabfee5b45348d05d918222a385314a431812aa5f5926aacf11560
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54107541"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Вхід для Windows 10 без використання пароля

Щоб не вводити пароль під час запуску Windows, радимо скористатися одним із параметрів безпечного входу Windows Hello, наприклад PIN-коду, розпізнавання обличчя або відбитків пальців, якщо вони доступні. Якщо ви справді хочете вимкнути безпечний вхід, див. наведені нижче інструкції "Автоматичний вхід Windows 10 входу".

**Захист Windows Hello і пароля облікового запису**

Перейдіть до **Настройки > Облікові > параметри входу** (або клацніть [тут).](ms-settings:signinoptions?activationSource=GetHelp) З'являться доступні параметри входу. Наприклад:

![Параметри входу.](media/sign-in-options.png)

Виберіть один із параметрів, щоб настроїти його. Під час наступного запуску Windows розблокування ви зможете використовувати новий параметр замість пароля. 

**Автоматичний вхід у Windows 10**

**Примітка.** Автоматичний вхід зручний, але впроваджує загрозу безпеці, особливо якщо ПК доступний кільком користувачам. 

1. Натисніть кнопку **Пуск** на панелі завдань.

2. Введіть **netplwiz і** натисніть клавішу Enter, щоб відкрити вікно "Облікові записи користувачів".

3. У **полі Облікові** записи користувачів виберіть обліковий запис, у який потрібно автоматично входити під час Windows запуску.

4. Зніміть прапорець "Користувачі повинні вводити ім'я користувача та пароль для використання цього комп'ютера".

    ![Користувачі повинні ввести ім'я користувача та пароль.](media/users-must-enter-username.png)

5. Натисніть кнопку **OK**. Вам буде запропоновано ввести та підтвердити пароль для вибраного облікового запису. Натисніть **кнопку OK,** щоб завершити. Під час Windows 10 буде автоматично ввійти у вибраний обліковий запис.
