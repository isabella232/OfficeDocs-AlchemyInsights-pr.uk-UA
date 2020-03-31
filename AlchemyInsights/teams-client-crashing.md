---
title: Клієнт Teams аварійно завершує роботу?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030759"
---
# <a name="teams-client-crashing"></a>Клієнт Teams аварійно завершує роботу?

Якщо клієнт Teams аварійно завершує роботу, виконайте наведені нижче дії.

- Якщо ви використовуєте класичну версію програми Teams, [переконайтеся, що її повністю оновлено](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Переконайтеся, що всі [діапазони URL- і IP-адрес Office 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) доступні.

- Увійдіть за допомогою облікового запису адміністратора та перегляньте [приладну дошку стану служби](https://docs.microsoft.com/office365/enterprise/view-service-health), щоб переконатись у відсутності перебоїв у роботі та зменшення продуктивності служби.

 - На останньому кроці ви можете спробувати очистити кеш клієнта Teams.

    1.  Повністю вийдіть із класичної програми Microsoft Team. Клацніть правою кнопкою миші **Teams** на піктограмі в системній треї, а потім виберіть **Вийти**. Ви також можете запустити диспетчер завдань і повністю вимкнути процес.

    2.  Відкрийте Файловий провідник і введіть %appdata%\Microsoft\teams.

    3.  У каталозі з’являться кілька наведених нижче папок.

         - Виберіть **Application Cache**, відкрийте папку Cache і видаліть із неї всі файли: %appdata%\Microsoft\teams\application cache\cache.

        - З папки **Blob_storage** видаліть усі файли: %appdata%\Microsoft\teams\blob_storage.

        - З папки **Cache** видаліть усі файли: %appdata%\Microsoft\teams\Cache.

        - З папки **databases** видаліть усі файли: %appdata%\Microsoft\teams\databases.

        - З папки **GPUCache** видаліть усі файли: %appdata%\Microsoft\teams\GPUcache.

        - З папки **IndexedDB** видаліть DB-файл: %appdata%\Microsoft\teams\IndexedDB.

        - З папки **Local Storage** видаліть усі файли: %appdata%\Microsoft\teams\Local Storage.

        - Насамкінець із папки **tmp** видаліть усі файли: %appdata%\Microsoft\teams\tmp.

    4. Перезапустіть клієнт Teams.
