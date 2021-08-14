---
title: SharePoint Проблеми з підключенням до конструктора
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: d55f7c1902bb623900fa74bdae70695b6e04ad84ce7b6ea314db614283ec436d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53942046"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Проблеми з підключенням до конструктора 

Якщо SharePoint із Дизайнером виникли проблеми з підключенням до SharePoint сайтів, спробуйте наведені нижче поширені рішення.

Крок 1. Переконайтеся, що SharePoint Дизайнер 2013 оновлено в SharePoint Designer з пакетом оновлень [1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) і оновлення від 2 серпня 2016 р. для [SharePoint Designer 2013.](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)



Крок 2. Очищення локальних файлів кеша

1. Закрийте SharePoint Дизайнер 2013.

2. Видаліть усі файли, знайдені в кожній із наведених нижче папок на локальному комп'ютері.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Відкрийте SharePoint Designer 2013 і введіть обліковий запис знову, щоб дізнатися, чи він працює.

Крок 3. [Активація сучасної автентифікації для Office 2013 на Windows пристроях.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)

Крок 4. Адміністратори  повинні дозволити користувацькі сценарії в параметрах Центру адміністрування SharePoint, щоб дозволити підключення конструктора SharePoint конструктора. Докладні [відомості див. в відео](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) Дозвіл і заборона користувацьких сценаріїв.


