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
ms.openlocfilehash: fc6731d5a7747bb4fc8d6cef1b6ac0045d11917d7f97abbb21eea9613b1b1aa2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093911"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Обмеження доступу в SharePoint або OneDrive

Є багато способів обмежити доступ до SharePoint онлайнових і OneDrive служб. Нижче наведено різні способи обмеження доступу. 

**Обмеження дозволів**

У SharePoint Online і OneDrive для бізнесу ми обмежуємо доступ до таких елементів, як сайти, файли та папки, надавши доступ лише цим групам або особам, які повинні мати доступ.

- [Настроювання дозволів для SharePoint списку або бібліотеки](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Настроювання SharePoint сайту](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Змінення дозволів для вкладеної папки](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Керування доступом із некерованих пристроїв](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Як SharePoint або глобальний адміністратор ви можете заблокувати або обмежити доступ до SharePoint і OneDrive вмісту з некерованіх пристроїв (які не гібридні приєдналися до служби AD або несумісні з ним в Intune).

**Обмеження мережевого розташування**

ІТ-адміністратор може керувати доступом до ресурсів SharePoint OneDrive на основі визначених мережевих розташунок, які ви довіряєте. Це також називається політикою на основі розташування. Докладні відомості див. в [статтях Керування доступом до служб SharePoint Online і OneDrive даних на основі мережевого розташування.](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Обмеження блокування сайту** 

У SharePoint Online ви можете заблокувати колекцію сайтів, тому ніхто не має доступу. Цей параметр установлено за допомогою Оболонки PowerShell [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) за допомогою властивості [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**Обмеження користувачів на створення сайтів і підсайтів**

Адміністратори SharePoint або глобальні адміністратори можуть дозволити користувачам створювати й адміністувати власні сайти SharePoint, визначати типи сайтів, які вони можуть створювати, і вказувати розташування сайтів. Докладні відомості див. в [розділі Керування створенням сайтів у SharePoint Online.](https://docs.microsoft.com/sharepoint/manage-site-creation)

