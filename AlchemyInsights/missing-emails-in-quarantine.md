---
title: Відсутні повідомлення електронної пошти в карантині
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673735"
---
# <a name="missing-emails-in-quarantine"></a>Відсутні повідомлення електронної пошти в карантині "

Адміністратори можуть [переглядати, вивільняти або видаляти ці повідомлення.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Щоб відкрити центр відповідності & безпеки, перейдіть до розділу [https://protection.office.com](https://protection.office.com/) . Щоб відкрити сторінку карантину безпосередньо, перейдіть до [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Шукати можна за такими значеннями:  

- **Ідентифікатор повідомлення**: глобальний унікальний ідентифікатор повідомлення. Якщо ви вибрали повідомлення в списку, то в області " **докладно** ", що Відкриється, ВІДОБРАЖАЄТЬСЯ значення **ідентифікатора повідомлення** . Адміністратори можуть використовувати [трасування повідомлень](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) , щоб знаходити повідомлення та відповідні значення ідентифікаторів повідомлень.
- **Адреса електронної пошти відправника**: адреса електронної пошти одного відправника.
- **Адреса електронної пошти одержувача**: адреса електронної пошти одного одержувача.
- **Тема**: використайте всю тему повідомлення. Пошук не враховує регістр.

Ввівши умови пошуку, натисніть кнопку Оновити, ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** щоб відфільтрувати результати.  

Командлети, які використовуються для перегляду та керування повідомленнями та файлами в карантині:
- [Видалення – карантин](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Експорт – карантин](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Початок-карантин](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Ознайомлювальну версію – карантин](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Зауважте, що цей командлет призначено лише для повідомлень, а не зловмисних файлів із АТФ для служби SharePoint Online, OneDrive для бізнесу або робочих груп.
- [Випуск – карантин](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)