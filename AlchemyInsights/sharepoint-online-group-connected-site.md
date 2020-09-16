---
title: Додавання групи до сайту SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771229"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Проблеми під час створення групи підключених сайтів у SharePoint

1. Деякі поширені проблеми виникають під час створення або повторного створення підключеного сайту групи.
Якщо ви видалили групу та його підключений сайт і хочете створити інший сайт з тією самою URL-адресою, потрібно остаточно видалити попередній сайт.

   - Завантажити [оболонку керування](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429) в "спо"
   - Докладні відомості про початок роботи з PowerShell наведено в статті [початок роботи з оболонкою керування службою SharePoint Online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Видаліть сайт із видалених сайтів за допомогою командлета [Remove-Spodeableedsite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell. PowerShell потрібен для остаточного видалення сайтів групи.

1. Якщо ви створюєте сайт, підключений до групи, і отримаєте попередження: **інша група з тим самим псевдонімом уже існує**, перевірте наявні групи в [центрі адміністрування Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Щоб вирішити цю проблему, видаліть наявну групу, якщо вона більше не потрібна, або створіть сайт з іншим призначенням псевдоніма.

1. Існує кілька способів створення та використання сучасних груп у службі SharePoint.

   - До групи Microsoft 365 можна підключити вже доступні сайти. Докладні відомості наведено в статті [підключення групи Microsoft 365 за допомогою інтерфейсу користувача SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Щоб створити сайт, підключений до групи Microsoft 365, потрібно створити [сайт групи](https://admin.microsoft.com/sharepoint).
