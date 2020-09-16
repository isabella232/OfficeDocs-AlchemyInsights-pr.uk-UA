---
title: Проблеми з підключенням до програми SharePoint Designer
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
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727192"
---
# <a name="sharepoint-designer-connection-issues"></a>Проблеми з підключенням до програми SharePoint Designer 

Якщо у програмі SharePoint Designer виникли проблеми з підключенням до сайтів SharePoint, спробуйте виконати наведені нижче поширені рішення.

Крок 1. Переконайтеся, що SharePoint Designer 2013 оновлюється за допомогою [служби SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) і [2 серпня 2016 оновлення для SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Крок 2: очищення локальних файлів кешу:

1. Закрийте програму SharePoint Designer 2013.

2. На локальному комп'ютері видаліть усі файли, знайдені в кожній із наведених нижче папок.

    - %AppData%\microsoft\ веб-сервер Extensions\Cache
    - %AppData%\microsoft\ SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Відкрийте програму SharePoint Designer 2013 і знову вкажіть обліковий запис, щоб дізнатися, чи це працює.

Крок 3: [Увімкнення сучасної автентифікації для Office 2013 на пристроях з ОС Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Крок 4: адміністратори повинні **дозволити настроюваний сценарій** у настройках центру адміністрування SharePoint, щоб дозволити підключення конструктора SharePoint. Дізнайтеся [, як дозволити або заборонити настроюваний сценарій](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) для отримання додаткових відомостей.


