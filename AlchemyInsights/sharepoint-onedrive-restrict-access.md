---
title: Обмеження доступу в SharePoint або OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 39aa8cd6e649eca4a1e196eeb589a825364d0977
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692786"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Обмеження доступу в SharePoint або OneDrive

Існує багато способів обмежити доступ до служб SharePoint Online/OneDrive. Ці різні методи обмеження доступу викладені нижче. 

**Обмеження доступу**

У SharePoint Online та OneDrive для бізнесу ми обмежуємо доступ до таких елементів, як сайти, файли та папки, лише надаючи доступ до цих груп/осіб, які мають доступ.

- [Настроювання дозволів для списку або бібліотеки SharePoint](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Настроювання дозволів сайту SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Змінення дозволів у вкладеній папці](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Керування доступом із некерованих пристроїв](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Як SharePoint або Глобальний адміністратор ви можете заблокувати або обмежити доступ до вмісту SharePoint і OneDrive з некерованих пристроїв (це не гібридні оголошення, які приєдналися або сумісні в InTune).

**Обмеження розташування мережі**

Як ІТ-адміністратор ви можете керувати доступом до ресурсів SharePoint і OneDrive на основі визначених мережевих розташувань, яким ви довіряєте. Це також відоме як політика на основі розташування. Для отримання додаткових відомостей зверніться до [керування доступом до SharePoint Online та OneDrive даних на основі мережного розташування](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Обмеження блокування сайту** 

У SharePoint Online у вас є можливість заблокувати колекцію сайтів, тому ніхто не має доступу. Це встановлено за допомогою PowerShell і [оболонки керування SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) , використовуючи властивість [Set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -локстан.

**Як заборонити користувачам створювати сайти або підсайти**

Як адміністратор SharePoint або Глобальний адміністратор ви можете дозволити користувачам створювати та адмініструвати власні сайти SharePoint, визначати, які сайти вони можуть створювати, і вказувати розташування сайтів. Для отримання додаткової інформації, будь ласка, дивіться [керування створенням сайту в SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

