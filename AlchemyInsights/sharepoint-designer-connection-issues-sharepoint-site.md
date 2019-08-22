---
title: SharePoint Designer і FTP-клієнти
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: a4aeaeaea5743c276b907c78317ff30f5610be81
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36508444"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer і FTP-клієнти 

Якщо SharePoint Designer переживає питання, підключення до сайтів SharePoint, будь ласка, спробуйте такі спільні рішення.

Крок 1: Переконайтеся, що SharePoint Designer 2013 оновлюється з [пакета оновлень 1 для SharePoint Designer](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) і [2 серпня 2016 оновлення для SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Крок 2: Очистити кеш локальних файлів:

1. Закрийте SharePoint Designer 2013.

2. На локальному комп'ютері видалити всі файли у кожному із таких папок.

    - %AppData%\Microsoft\Web сервер Extensions\Cache
    - %AppData%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Відкрити SharePoint Designer 2013 і введіть обліковий запис знову, щоб побачити, якщо вона працює.

Крок 3: [ввімкнення сучасних автентифікації для Office 2013 на пристроях Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

Крок 4: Адміністратори повинні **Дозволити користувацький скрипт** в настройках центру адміністрування SharePoint дозволити підключення застосунку SharePoint Designer. Див [дозволити або заборонити власний сценарій](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) для отримання додаткової інформації.


