---
title: Усунення несправностей, пов'язаних із аварійно заверш
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
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826220"
---
# <a name="troubleshoot-onedrive-crashes"></a>Усунення несправностей, пов'язаних із аварійно заверш

Якщо OneDrive неодноразово аварійно завершує роботу, спробуйте виконати наведені нижче дії з виправлення неполадок.

**Переконайтеся, що розділи реєстру не настроєно.**

1. За допомогою редактора реєстру перейдіть до HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Якщо disableFileSyncNGSC встановлено та встановлено значення 1, відкрийте ключ і змініть значення на 0.
3. Вручну запустіть OneDrive у меню "Пуск" ![Натисніть клавішу Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), введіть OneDrive у полі пошуку, а потім клацніть класичну програму OneDrive.

**Скидання OneDrive**

Примітки.

- Під час скидання OneDrive роз'єднує всі наявні підключення для синхронізації (включно з особистим обліковим записом OneDrive, якщо його налаштовано).
- Ви не втратите файли або дані, якщо скинете параметри OneDrive на комп'ютері.

**Щоб скинути параметри OneDrive:**

1. Відкрийте діалогове вікно "Виконати", натиснувши клавіші Windows і R.
2. Введіть %localappdata%\Microsoft\OneDrive\onedrive.exe /reset і натисніть кнопку OK. Коротко може з'явитися вікно командного рядка.
3. Вручну запустіть OneDrive у меню "Пуск" ![Натисніть клавішу Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), введіть OneDrive у полі пошуку, а потім клацніть класичну програму OneDrive.

Примітки.

- Якщо ви синхронізувати лише певні папки до скидання, це потрібно зробити ще раз після синхронізації. Докладні відомості див. в розділі Вибір папок [OneDrive, які потрібно синхронізувати з](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   комп'ютером.
- Це потрібно зробити для особистого сховища OneDrive і "OneDrive для бізнесу".