---
title: Додавання групи до SharePoint сайту
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200004"
- "5766"
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 8166c2a19e5849de6caace4eea0fee5866f5adc3bfc2c483f18fc788c1bf2fa9
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/11/2021
ms.locfileid: "57897737"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>Поширені проблеми під час створення сайту, підключеного до SharePoint

1. Якщо ви видалили групу та підключений до неї сайт і хочете створити інший сайт із тією ж URL-адресою, вам доведеться остаточно видалити попередній сайт.

   - Завантажити [оболонку керування SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Докладні відомості про початок роботи з PowerShell див. в SharePoint [Online Management Shell.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)
   - Видаліть сайт із видалених сайтів за допомогою командлета PowerShell [Remove-SPODeletedSite.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Щоб остаточно видалити сайти групи, потрібна оболонка PowerShell.

1. Якщо ви створюєте сайт, підключений до групи, і отримуєте **попередження:** Інша група з таким самим псевдонімом уже існує, перевірте наявні групи в [Центр адміністрування Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Щоб вирішити цю проблему, видаліть наявну групу, якщо вона більше не потрібна, або створіть сайт з іншим призначеним псевдонімом.

1. Існує кілька способів створення та використання сучасних груп із SharePoint.

   - До групи можна підключити наявні Microsoft 365 сайтів. Докладні відомості [див. в Підключення групі Microsoft 365 за допомогою SharePoint інтерфейсу користувача.](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)
   - Щоб створити Microsoft 365, знадобиться створити сайт [групи.](https://admin.microsoft.com/sharepoint)
