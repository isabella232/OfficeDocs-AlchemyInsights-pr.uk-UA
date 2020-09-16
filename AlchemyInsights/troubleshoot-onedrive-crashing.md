---
title: Усунення несправностей у OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665019"
---
# <a name="troubleshoot-onedrive-crashes"></a>Усунення несправностей у OneDrive

Якщо не вдається повторно завершити роботу, виконайте наведені нижче дії з виправлення неполадок.

**Переконайтеся, що розділи реєстру не настроєно:**

1. У редакторі реєстру перейдіть до HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive
2. Якщо DisableFileSyncNGSC присутній і настроєно на 1, відкрийте ключ і змініть значення на 0.
3. Запуск OneDrive вручну за допомогою переходу на початок ![Натисніть клавішу Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), у полі пошуку введіть OneDrive, а потім клацніть піктограму для настільних комп'ютерів у програмі OneDrive.

**Скидання "OneDrive":**

Нотаток

- Скидання "OneDrive" відключає всі поточні зв'язки синхронізації (включно з особистим "OneDrive", якщо його настроєно).
- Ви не втратите файли або дані, скинувши OneDrive на вашому комп'ютері.

**Щоб скинути його, виконайте наведені нижче дії.**

1. Відкрийте діалогове вікно "виконати", натиснувши клавіші Windows і R.
2. Введіть% localappdata% \Microsoft\OneDrive\onedrive.exe/Reset. і натисніть кнопку OK. У вікні командного рядка може відображатися короткий час.
3. Запуск OneDrive вручну за допомогою переходу на початок ![Натисніть клавішу Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), у полі пошуку введіть OneDrive, а потім клацніть піктограму для настільних комп'ютерів у програмі OneDrive.

Нотаток

- Якщо ви вирішили синхронізувати лише деякі папки перед скиванням, потрібно буде виконати цю дію знову після завершення синхронізації. Дізнайтеся [, які папки OneDrive синхронізуються з комп'ютером,](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)щоб отримати   докладні відомості.
- Вам потрібно буде виконати це для особистого "OneDrive" та "OneDrive для бізнесу".