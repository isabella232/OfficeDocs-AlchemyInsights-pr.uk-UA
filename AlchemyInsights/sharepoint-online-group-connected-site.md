---
title: Додавання групи до сайту SharePoint
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 423db4e5bbb85e75aee3548d5b6b46a64ebc6fa0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750541"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>Проблеми під час створення або групи підключених сайтів у SharePoint Online

Існує кілька поширених проблем, які виникають під час створення або Повторне створення групи, підключеного сайту.

 Якщо ви видалили групу та її підключений сайт і бажаєте створити інший сайт з однаковою URL-адресою, потрібно остаточно видалити попередній сайт.

Завантажити [оболонку керування спо](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Щоб отримати додаткові відомості про початок роботи з PowerShell, див. [початок роботи з оболонки керування SharePoint Online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Видалення сайту з видалених сайтів за допомогою командлета [видалення-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell.

Якщо ви створюєте сайт групи, підключений і отримати попередження іншу групу з таким самим псевдонімом вже існує, перевірте наявні групи з [Office 365 з центру адміністрування](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Щоб вирішити цю проблему, видаліть наявну групу, якщо вона більше не потрібна, або створіть сайт з іншим псевдонімом.

Існують різні способи створення та використання сучасних груп з SharePoint.

Можна підключити наявні сайти до групи Office 365. Для отримання додаткових відомостей див. [підключення групи Office 365 за допомогою користувача SharePoint ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Щоб створити групу Office 365, підключений сайт, потрібно створити сайт групи. Для отримання додаткових відомостей див. [Створення сайту групи в SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

