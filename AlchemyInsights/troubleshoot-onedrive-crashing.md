---
title: Усунення несправностей OneDrive аварійно завершує роботу
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: d5982bafbb8aaa1d240a34c071efe37e92c2ec5c5170dc59337df9a5435e22e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53921028"
---
# <a name="troubleshoot-onedrive-crashes"></a>Усунення несправностей OneDrive аварійно завершує роботу

Якщо OneDrive аварійно завершує роботу, спробуйте виконати такі дії з виправлення неполадок:

**Переконайтеся, що розділи реєстру не настроєно.**

1. За допомогою редактора реєстру перейдіть до HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Якщо disableFileSyncNGSC встановлено та встановлено значення 1, відкрийте ключ і змініть значення на 0.
3. Запуск вручну OneDrive в меню "Пуск" ![Натисніть клавішу Windows.](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), OneDrive у полі пошуку, а потім клацніть піктограму OneDrive класичній програмі.

**Скидання OneDrive:**

Примітки.

- Скидання OneDrive від'єднує всі наявні підключення для синхронізації (включно з OneDrive, якщо їх налаштовано).
- Ви не втратите файли або дані, скинувши параметри OneDrive комп'ютері.

**Щоб скинути OneDrive:**

1. Відкрийте діалогове вікно Виконати, натиснувши клавіші Windows R.
2. Введіть %localappdata%\Microsoft\OneDrive\onedrive.exe /reset і натисніть кнопку OK. Коротко може з'явитися вікно командного рядка.
3. Запуск вручну OneDrive в меню "Пуск" ![Натисніть клавішу Windows.](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), OneDrive у полі пошуку, а потім клацніть піктограму OneDrive класичній програмі.

Примітки.

- Якщо ви синхронізувати лише певні папки до скидання, це потрібно зробити ще раз після синхронізації. Докладні [відомості див. OneDrive в](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)розділі Вибір папок, які потрібно синхронізувати з   комп'ютером.
- Це потрібно зробити для особистих облікових OneDrive і OneDrive для бізнесу.