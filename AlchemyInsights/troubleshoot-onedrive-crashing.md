---
title: Усунення несправностей OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/15/2020
ms.locfileid: "44749241"
---
# <a name="troubleshoot-onedrive-crashes"></a>Усунення несправностей OneDrive

Якщо OneDrive кілька разів аварійно завершує роботу, спробуйте виконати такі дії:

**Переконайтеся, що розділи реєстру не встановлено:**

1. За допомогою редактора реєстру, перейдіть до HKEY_LOCAL_MACHINE \ програмне забезпечення\price\micti
2. Якщо в наявності є 1, відкрийте ключ і змініть значення на 0, якщо він є.
3. Запустіть OneDrive вручну, перейшовши на початок ![Натисніть клавішу Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), у полі пошуку введіть OneDrive, а потім клацніть програму OneDrive для настільних комп'ютерів.

**Скинути OneDrive:**

Нотатки:

- Скидання настройок OneDrive припиняється з усіма існуючими синхронізованими підключеннями (включно з особистими OneDrive у разі настроювання).
- Ви не втратите файли або дані, відновивши OneDrive на комп'ютері.

**Щоб скинути OneDrive:**

1. Щоб відкрити діалогове вікно запуску, натисніть клавішу Windows і R.
2. Введіть% localappdata% \Microsoft\OneDrive\onedrive.exe/Reset і натисніть OK. Вікно командного рядка може здатися коротко.
3. Запустіть OneDrive вручну, перейшовши на початок ![Натисніть клавішу Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), у полі пошуку введіть OneDrive, а потім клацніть програму OneDrive для настільних комп'ютерів.

Нотатки:

- Якщо ви вирішили синхронізувати лише деякі папки перед скиданням, вам потрібно буде зробити це знову після завершення синхронізації. Дізнайтеся [, як вибрати папки OneDrive для синхронізації з комп'ютером](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   для отримання додаткових відомостей.
- Вам потрібно буде завершити це для вашого особистого OneDrive і OneDrive для бізнесу.