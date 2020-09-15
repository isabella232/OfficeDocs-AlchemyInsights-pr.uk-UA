---
title: Обмеження доступу в SharePoint або OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700476"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Обмеження доступу в SharePoint або OneDrive

Існує багато способів обмежити доступ до служб SharePoint Online або OneDrive. Нижче наведені різні методи обмеження доступу. 

**Обмеження дозволів**

У службі SharePoint Online і "OneDrive для бізнесу" ми обмежуємо доступ до таких елементів, як сайти, файли та папки, лише надаючи доступ до цих груп або осіб, які мають доступ.

- [Настроювання дозволів для списку або бібліотеки SharePoint](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Настроювання дозволів на сайт SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Змінення дозволів у вкладеній папці](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Керування доступом із некерованих пристроїв](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Як служба SharePoint або Глобальний адміністратор, ви можете блокувати або обмежувати доступ до вмісту SharePoint і OneDrive з некерованих пристроїв (ті, що не є гібридним ОГОЛОШЕННЯМ, до яких приєдналися або сумісні в Inune).

**Обмеження мережного розташування**

Як ІТ-адміністратор можна керувати доступом до ресурсів SharePoint і OneDrive на основі визначених мережевих розташувань, які ви довіряєте. Цей параметр також відомий як політика на основі розташування. Докладні відомості наведено в статті [керування доступом до даних SharePoint Online і OneDrive на основі мережного розташування](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location) .

**Обмеження блокування сайту** 

У службі SharePoint Online ви маєте можливість заблокувати колекцію сайтів, щоб мати доступ до них. Цей параметр настроєно через PowerShell і [оболонку керування SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) за допомогою властивості [Set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.

**Обмеження користувачів зі створення сайтів і підсайтів**

Адміністратор SharePoint або Глобальний адміністратор дає змогу користувачам створювати та адмініструвати власні сайти SharePoint, визначати типи сайтів, які вони можуть створювати, а також визначати розташування сайтів. Докладні відомості наведено [в статті керування створенням сайтів у службі SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

