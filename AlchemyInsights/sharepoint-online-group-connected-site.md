---
title: Додати групу на сайті SharePoint
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 6aea12d44a44a3e11eaf3fb1bd47ff3e9dbfd9e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507868"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>Проблеми під час створення або групу пов'язаних сайтів в SharePoint Online

Є кілька поширених проблем під час створення або Повторне створення групи пов'язаних сайтів.

 Якщо ви видалили групи та пов'язаних сайт і хотіли б створити інший сайт з той самий URL, потрібно буде остаточно видалити попередній вузол.

Завантажити [оболонки керування спо](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Для отримання додаткової інформації на знайомство з powershell див [знайомство з SharePoint онлайн оболонки керування](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Видалення сайту з видалено веб-сайтів за допомогою командлета powershell [Видалити SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .

Якщо ви створюєте групи пов'язаних сайт і отримувати попередження, інша група з же псевдонімом вже існує, перевірте існуючих груп з [Office 365 з центру адміністрування](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Щоб вирішити цю проблему, видалення наявної групи, якщо він більше не потрібна або створити сайт з різними псевдонім призначено.

Існують різні способи, щоб створити і використовувати сучасні групи з SharePoint.

Наявних сайтів можна підключити до Office 365 групи. Для отримання додаткової інформації див [підключення служби Office 365 групи, за допомогою ineterface користувача SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Створити Office 365 Група пов'язаних сайт, потрібно буде створити сайт групи. Для отримання додаткової інформації дивіться [Створення сайту групи в SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

