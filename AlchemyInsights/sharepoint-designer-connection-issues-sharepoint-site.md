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
ms.openlocfilehash: 7451cfe957545537298f57feb5b47bd6d43cddbf
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716912"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer і FTP-клієнти 

<p>Якщо SharePoint Designer переживає питання, підключення до сайтів SharePoint, будь ласка, спроба такі спільні рішення.</p> <p><strong>Крок 1:</strong> <strong>Перевірити SharePoint Designer оновлюється&nbsp; </strong></p> <ul> <li><a href="https://www.microsoft.com/en-us/download/details.aspx?id=35491">SharePoint Designer 2013</a></li> <li><a href="https://support.microsoft.com/en-us/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1">SharePoint Designer пакета оновлень 1 (SP1)</a></li> <li><a href="https://support.microsoft.com/en-us/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721">Оновлення для SharePoint Designer 2013 (KB3114721)</a></li> </ul> <p><strong>Крок 2:</strong> <strong>Очистити кеш локальних файлів</strong>&nbsp;</p> <ol> <li style="font-weight: 400;">Закрийте SharePoint Designer 2013.&nbsp;</li> <li style="font-weight: 400;">На локальному комп'ютері перейдіть до таких папок, щоб видалити кешованих файлів.&nbsp;</li> <li style="font-weight: 400;">Натисніть <strong>Пуск -&gt; запустити</strong> а видаліть усі файли, знайдені під кожним на нижче розташуваннях.&nbsp;<br /><br />%AppData%\Microsoft\Web сервер Extensions\Cache<br />%AppData%\Microsoft\SharePoint Designer\ProxyAssemblyCache<br />%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</li> <li style="font-weight: 400;">Відкрити SharePoint Designer 2013 і введіть обліковий запис знову, щоб побачити, якщо вона працює.</li> </ol> <p><strong>Крок 3:</strong> <a href="https://docs.microsoft.com/en-us/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=%252fen-us%252farticle%252fEnable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&amp;view=o365-worldwide"> <strong>Ввімкнення сучасних автентифікації для Office 2013 на пристроях Windows</strong></a>&nbsp;</p> <p><strong>Крок 4:</strong> <strong>Адміністратори повинні дозволити користувацький скрипт дозволити підключення застосунку SharePoint Designer</strong>.</p> <p>Докладно процедуру, приклади і міркування в розділі <a href="https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script">дозволити або заборонити власний сценарій</a>.&nbsp;</p>


