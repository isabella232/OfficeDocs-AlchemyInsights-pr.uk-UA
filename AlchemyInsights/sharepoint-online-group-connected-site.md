---
title: Додавання групи до сайту SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 5dab9fce935936898927afd55f8f6e9260249157
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582832"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Проблеми під час створення групи, підключений сайт у програмі SharePoint

1. Деякі поширені проблеми, які виникають під час створення або Повторне створення групи, підключений сайт.
Якщо ви видалили групу та її підключений сайт і бажаєте створити інший сайт з однаковою URL-адресою, потрібно остаточно видалити попередній сайт.

   - Завантажити [оболонку керування спо](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Щоб отримати додаткові відомості про початок роботи з PowerShell, [див.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)
   - Видалення сайту з видалених сайтів за допомогою командлета [видалення-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell. PowerShell потрібно остаточно видалити групи сайтів.

1. Якщо створюється Група підключених сайтів і з'являється попередження: **ще одна група з таким самим псевдонімом уже існує**, перевірте наявні групи з [центру адміністрування Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Щоб вирішити цю проблему, видаліть наявну групу, якщо вона більше не потрібна, або створіть сайт з іншим псевдонімом.

1. Існують різні способи створення та використання сучасних груп з SharePoint.

   - Можна підключити наявні сайти до групи Microsoft 365. Для отримання додаткових відомостей див. [підключення групи Microsoft 365 за допомогою інтерфейсу користувача SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Щоб створити групу Microsoft 365, підключений сайт, потрібно створити [сайт групи](https://admin.microsoft.com/sharepoint).
