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
ms.openlocfilehash: e7bfabe1555bb94e915f8544d460deecce6171be
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770372"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="6b82c-102">Проблеми під час створення групи, підключений сайт у програмі SharePoint</span><span class="sxs-lookup"><span data-stu-id="6b82c-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="6b82c-103">Деякі поширені проблеми, які виникають під час створення або Повторне створення групи, підключений сайт.</span><span class="sxs-lookup"><span data-stu-id="6b82c-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="6b82c-104">Якщо ви видалили групу та її підключений сайт і бажаєте створити інший сайт з однаковою URL-адресою, потрібно остаточно видалити попередній сайт.</span><span class="sxs-lookup"><span data-stu-id="6b82c-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="6b82c-105">Завантажити [оболонку керування спо](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="6b82c-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="6b82c-106">Щоб отримати додаткові відомості про початок роботи з PowerShell, [див.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)</span><span class="sxs-lookup"><span data-stu-id="6b82c-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="6b82c-107">Видалення сайту з видалених сайтів за допомогою командлета [видалення-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6b82c-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="6b82c-108">PowerShell потрібно остаточно видалити групи сайтів.</span><span class="sxs-lookup"><span data-stu-id="6b82c-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="6b82c-109">Якщо створюється Група підключених сайтів і з'являється попередження: **ще одна група з таким самим псевдонімом уже існує**, перевірте наявні групи з [Office 365 з центру адміністрування](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="6b82c-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="6b82c-110">Щоб вирішити цю проблему, видаліть наявну групу, якщо вона більше не потрібна, або створіть сайт з іншим псевдонімом.</span><span class="sxs-lookup"><span data-stu-id="6b82c-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="6b82c-111">Існують різні способи створення та використання сучасних груп з SharePoint.</span><span class="sxs-lookup"><span data-stu-id="6b82c-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="6b82c-112">Можна підключити наявні сайти до групи Office 365.</span><span class="sxs-lookup"><span data-stu-id="6b82c-112">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="6b82c-113">Для отримання додаткових відомостей див. [підключення групи Office 365 за допомогою інтерфейсу користувача SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="6b82c-113">For more info, see [Connect an Office 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="6b82c-114">Щоб створити групу Office 365, підключений сайт, потрібно створити [сайт групи](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="6b82c-114">To create an Office 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
