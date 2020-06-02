---
title: Проблеми з підключенням до конструктора SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 01ccc6bc28148f397fb6cd2b7a0eaaeb5b51973f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511565"
---
# <a name="sharepoint-designer-connection-issues"></a>Проблеми з підключенням до конструктора SharePoint 

Якщо SharePoint Designer переживає проблеми з підключенням до сайтів SharePoint, спробуйте скористатися такими загальними рішеннями.

Крок 1: переконайтеся, що SharePoint Designer 2013 оновлено [SharePoint Designer з пакетом оновлень 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) і [2 серпня 2016 оновлення для SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Крок 2: очистіть локальні файли кешу:

1. Закрийте SharePoint Designer 2013.

2. На локальному комп'ютері видаліть усі файли, знайдені в кожній з таких папок.

    - %Appind%\mempice\веб-сервер розширення \ кеш
    - %Appind%\mempice\sharepoint Designer\ProxyAssemblyCache
    - % Userпрофільні%\appind\locm

3. Відкрийте SharePoint Designer 2013 і знову введіть обліковий запис, щоб побачити, чи працює він.

Крок 3: [Увімкнення сучасних автентифікації для Office 2013 на пристроях Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Крок 4: адміністраторам потрібно **дозволити користувацький скрипт** у настройках центру адміністрування SharePoint, щоб дозволити підключення конструктора SharePoint. Щоб отримати додаткові відомості [,](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) див.


