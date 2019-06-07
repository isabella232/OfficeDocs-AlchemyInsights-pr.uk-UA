---
title: Рівні дозволів на сайті SharePoint
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760713"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer і FTP-клієнти 

Якщо SharePoint Designer переживає питання, підключення до сайтів SharePoint, будь ласка, спроба такі спільні рішення.

Крок 1: Перевірте, чи оновлено SharePoint Designer.

- [SharePoint Designer 2013](https://www.microsoft.com/download/details.aspx?id=35491)

- [SharePoint Designer пакета оновлень 1 (SP1)](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [Оновлення для SharePoint Designer 2013 (KB3114721)](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

Крок 2: Очистити кеш локальних файлів

- Закрийте SharePoint Designer 2013.

- На локальному комп'ютері перейдіть до таких папок, щоб видалити кешованих файлів.

- Натисніть кнопку Пуск, виконати і видалити всі файли, знайти під кожним з в нижче розташуваннях.

Сервер %AppData%\Microsoft\Web Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

Відкрити SharePoint Designer 2013 і введіть обліковий запис знову, щоб побачити, якщо вона працює.

Крок 3: [ввімкнення сучасних автентифікації для Office 2013 на пристроях Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)

Крок 4: Адміністратори повинні дозволити користувацький скрипт дозволити підключення застосунку SharePoint Designer.

Докладно процедуру, приклади і міркування в розділі [дозволити або заборонити власний сценарій](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


