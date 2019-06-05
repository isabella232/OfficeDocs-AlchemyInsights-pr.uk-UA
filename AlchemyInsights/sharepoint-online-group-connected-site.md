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
ms.openlocfilehash: 352bad1b8fe219f95a37c9ac268c6c4dd8801dfc
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719502"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>Створити групу пов'язаних сайт у SharePoint Online

<p><strong>Є кілька поширених проблем під час створення або Повторне створення групи пов'язаних сайтів.&nbsp;</strong></p>  <p>1.Якщо ви видалили групи та пов'язаних сайт і хотіли б створити інший сайт з той самий URL, потрібно буде остаточно видалити попередній вузол.</p>  <ul>  <li>Завантажити <a title="оболонку керування спо" href="https://support.office.com/en-ie/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429">SPO Management Shell</a> - для отримання додаткової інформації на знайомство з powershell див <a title="знайомитесь з онлайн оболонки керування SharePoint" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Початок роботи з SharePoint онлайн Management Shell</a>. <br /><br /></li>  <li>Видалення сайту з видалено сайтів, що використовують в <a title="видалити SPODeletedSite" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Видалити SPODeletedSite</a> командлета powershell.</li>  </ul>  <p>Якщо ви створюєте групи пов'язаних сайт і отримувати попередження, <strong>інша група з же псевдонімом вже існує</strong>, перевірте існуючих груп з на <a title="Office 365 з центру адміністрування" href="https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups">Office 365 з центру адміністрування</a>. Щоб вирішити цю проблему, видалення наявної групи, якщо він більше не потрібна або створити сайт з різними псевдонім призначено.&nbsp;</p>  <p><strong>Існують різні способи, щоб створити і використовувати сучасні групи з SharePoint.&nbsp;</strong></p>  <ol>  <li>Наявних сайтів можна підключити до Office 365 групи. Для отримання додаткової інформації див <a title="підключення служби Office 365 групи, за допомогою SharePoint користувача ineterface" href="https://docs.microsoft.com/en-us/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface">Підключення служби Office 365 групи, за допомогою SharePoint користувача ineterface</a>.</li>  <li>Створити Office 365 Група пов'язаних сайт, потрібно буде створити сайт групи. Для отримання додаткової інформації див <a title="створити сайт групи SharePoint, у" href="https://support.office.com/en-us/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d">Створити сайт групи SharePoint.</a></li>  </ol>

