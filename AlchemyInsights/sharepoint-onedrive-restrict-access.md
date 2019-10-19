---
title: Обмеження доступу в SharePoint або OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/18/2019
ms.locfileid: "36750685"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Обмеження доступу в SharePoint або OneDrive

Існує багато способів обмежити доступ до служб SharePoint Online/OneDrive. Ці різні методи обмеження доступу викладені нижче. 

**Обмеження доступу**

У SharePoint Online та OneDrive для бізнесу ми обмежуємо доступ до таких елементів, як сайти, файли та папки, лише надаючи доступ до цих груп/осіб, які мають доступ.

- [Настроювання дозволів для списку або бібліотеки SharePoint](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Настроювання дозволів сайту SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Змінення дозволів у вкладеній папці](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Керування доступом із некерованих пристроїв](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

У SharePoint або Global Admin в Office 365 можна заблокувати або обмежити доступ до вмісту SharePoint і OneDrive з некерованих пристроїв (не сумісні або несумісні оголошення в InTune).

**Обмеження розташування мережі**

Як ІТ-адміністратор ви можете керувати доступом до ресурсів SharePoint і OneDrive на основі визначених мережевих розташувань, яким ви довіряєте. Це також відоме як політика на основі розташування. Для отримання додаткових відомостей зверніться до [керування доступом до SharePoint Online та OneDrive даних на основі мережного розташування](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Обмеження блокування сайту** 

У SharePoint Online у вас є можливість заблокувати колекцію сайтів, тому ніхто не має доступу. Це встановлено за допомогою PowerShell і [оболонки керування SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) , використовуючи властивість [Set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -локстан.

**Як заборонити користувачам створювати сайти або підсайти**

Як адміністратор SharePoint або Office 365 Global Admin ви можете дозволити користувачам створювати та адмініструвати власні сайти SharePoint, визначати, які сайти вони можуть створювати, і вказати розташування сайтів. Для отримання додаткової інформації, будь ласка, дивіться [керування створенням сайту в SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

