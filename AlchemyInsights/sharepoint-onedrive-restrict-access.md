---
title: Обмеження доступу в SharePoint або OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 5101366ff65f477c19b9c7f2c0d7065cf88501b0
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/05/2019
ms.locfileid: "34735163"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Обмеження доступу в SharePoint або OneDrive

Є багато способів для обмеження доступу до служб SharePoint на сайті/OneDrive. Ці різні методи обмеження доступу викладені нижче. 

Обмеження дозволів

У SharePoint Online і OneDrive для бізнесу ми заборонити доступ до пунктам, як сайти, файли та папки, тільки надання доступу до цих груп/особи, які повинні мати доступ.

[Настроювання дозволів для списку або бібліотеки](https://support.office.com/en-us/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

[Настроїти дозволи сайту SharePoint](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions)

[Змінити дозволи на вкладену папку](https://support.office.com/en-us/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

[Керування доступом від некерованих пристроїв](https://docs.microsoft.com/en-us/sharepoint/control-access-from-unmanaged-devices)

SharePoint або глобального адміністратора, у службі Office 365, ви можете блокувати або обмежити доступ до SharePoint і OneDrive вміст від некерованих пристроїв (ті не гібридних оголошення об'єднуваних або сумісний в Intune).

Обмеження розташування мережі

Як адміністратор можна контролювати доступ до SharePoint і OneDrive ресурсів на основі визначених мережних розташуваннях, яким ви довіряєте. Це також відомо як місцезнаходженням політики. Для отримання додаткової інформації будь ласка, дивіться [керування доступом до SharePoint Online і OneDrive даних на основі мережне розташування](https://docs.microsoft.com/en-us/sharepoint/control-access-based-on-network-location)

Сайт блокування обмеження 

У SharePoint на сайті у вас є можливість блокування колекції сайтів, так що ніхто не має доступу. Це встановити за допомогою PowerShell і [SharePoint онлайн оболонки керування](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) властивістю - LockState [Set-SPOSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) .

Заборонити користувачам створення сайтів чи дочірні сайти

Як адміністратор SharePoint або Office 365 глобального адміністратора, можна дозволити користувачам створювати і управляти свої власні сайти SharePoint, визначити, якого роду сайти вони можуть створити і вкажіть розташування сайтів. Для отримання додаткової інформації будь ласка, дивіться [Створення сайту керування в SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/manage-site-creation)

