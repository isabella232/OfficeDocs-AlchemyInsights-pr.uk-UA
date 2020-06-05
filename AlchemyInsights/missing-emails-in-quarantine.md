---
title: Відсутні електронні листи в карантин
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569564"
---
# <a name="missing-emails-in-quarantine"></a>Відсутні електронні листи в карантин "

Адміністратори можуть [переглядати, випускати або видаляти ці повідомлення.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Щоб відкрити центр дотримання безпеки &, перейдіть до [https://protection.office.com](https://protection.office.com/) . Щоб відкрити сторінку карантину безпосередньо, перейдіть до [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Можна виконати пошук за такими значеннями:  

- **Ідентифікатор повідомлення**: глобальний унікальний ідентифікатор повідомлення. Якщо у списку вибрано повідомлення, значення **ідентифікатора повідомлення** відобразиться в спливаючому вікні **відомостей** , що з'явиться. Адміністратори можуть використовувати [трасування повідомлень](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) , щоб знайти повідомлення та їх ВІДПОВІДНІ значення ідентифікатора повідомлення.
- **Адреса електронної пошти відправника**: адреса електронної пошти одного відправника.
- **Адреса електронної пошти одержувача**: адреса електронної пошти одного одержувача.
- **Тема**: використовуйте весь об'єкт повідомлення. Пошук не враховується з урахуванням регістру.

Після введення критеріїв пошуку натисніть ![ кнопку Оновити ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **оновлення** , щоб відфільтрувати результати.  

Командлети, які використовуються для перегляду та керування повідомленнями та файлами в карантин:
- [Видалити-карантин](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Експорт-карантин](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Отримати-карантин](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Попередній перегляд-карантин](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Зверніть увагу, що цей командлет призначений лише для повідомлень, а не зловмисних файлів з АТФ для SharePoint Online, OneDrive, для бізнесу або команди.
- [Реліз-карантин](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)