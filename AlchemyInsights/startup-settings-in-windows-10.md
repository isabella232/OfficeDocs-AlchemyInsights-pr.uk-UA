---
title: Параметри запуску в Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: 526b92013f26675b5bf42077271ae7dc7003af31fa8f605d76aea92e0ccabfa1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53909847"
---
# <a name="startup-settings-in-windows-10"></a>Параметри запуску в Windows 10

**Змінення програм, які запускаються автоматично під час запуску системи**

1. Перейдіть до [Настройки > Програми > запуск](ms-settings:startupapps?activationSource=GetHelp).

2. Переконайтеся, що будь-яку програму, яку потрібно запускати під час запуску, увімкнуто .

**Додавання програми для автоматичного запуску**

1. Натисніть кнопку **Пуск** і знайдіть програму, яку потрібно запустити під час запуску.

2. Клацніть програму правою кнопкою миші, виберіть пункт **Додатково**, а потім виберіть **пункт Відкрити розташування файлу.** Відкриється розташування, у якому збережено ярлик програми. Якщо для параметра "Відкрити розташування файлу" немає параметра, це означає, що програма не може запуститися під час запуску.

3. Відкрийте розташування файлу, натисніть клавішу **Windows + R**, введіть **shell:startup**, а потім натисніть кнопку **OK.** Відкриється папка автозавантаження.

4. Скопіюйте та вставте ярлик програми з розташування файлу до папки автозавантаження.

**Додаткові параметри запуску (зокрема, Сейф режим, параметри UEFI та завантаження з іншого пристрою)**

1. Збережіть свою роботу та закрийте всі відкриті документи, оскільки ці дії перезавантажать комп'ютер.

2. Перейдіть до [Настройки > Оновлення & безпеки > відновлення.](ms-settings:recovery?activationSource=GetHelp)

3. У розділі **Додаткові параметри запуску натисніть** кнопку **Перезавантажити зараз.** 

4. Коли ПК перезавантажиться, на екрані Виберіть варіант:

    - Щоб завантажити його з пристрою, наприклад USB-носія, натисніть **кнопку "Використовувати пристрій".**

    - Щоб ввести параметри UEFI (інколи це називається налаштуванням BIOS), виберіть посилання Виправлення неполадок із > додатковими параметрами > мікропрограми **UEFI Настройки**. 

    - Щоб ввести Сейф або змінити додаткові параметри запуску, клацніть Виправлення неполадок > додаткових параметрів **> та** Настройки натисніть кнопку **Перезапустити.** Можливо, знадобиться ввести [ключ відновлення BitLocker.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key) Коли ПК знову перезавантажиться, клацніть потрібну настройку запуску.