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
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="bf718-102">Проблеми під час створення або групу пов'язаних сайтів в SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="bf718-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="bf718-103">Є кілька поширених проблем під час створення або Повторне створення групи пов'язаних сайтів.</span><span class="sxs-lookup"><span data-stu-id="bf718-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="bf718-104">Якщо ви видалили групи та пов'язаних сайт і хотіли б створити інший сайт з той самий URL, потрібно буде остаточно видалити попередній вузол.</span><span class="sxs-lookup"><span data-stu-id="bf718-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="bf718-105">Завантажити [оболонки керування спо](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="bf718-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="bf718-106">Для отримання додаткової інформації на знайомство з powershell див [знайомство з SharePoint онлайн оболонки керування](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="bf718-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="bf718-107">Видалення сайту з видалено веб-сайтів за допомогою командлета powershell [Видалити SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="bf718-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="bf718-108">Якщо ви створюєте групи пов'язаних сайт і отримувати попередження, інша група з же псевдонімом вже існує, перевірте існуючих груп з [Office 365 з центру адміністрування](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="bf718-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="bf718-109">Щоб вирішити цю проблему, видалення наявної групи, якщо він більше не потрібна або створити сайт з різними псевдонім призначено.</span><span class="sxs-lookup"><span data-stu-id="bf718-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="bf718-110">Існують різні способи, щоб створити і використовувати сучасні групи з SharePoint.</span><span class="sxs-lookup"><span data-stu-id="bf718-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="bf718-111">Наявних сайтів можна підключити до Office 365 групи.</span><span class="sxs-lookup"><span data-stu-id="bf718-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="bf718-112">Для отримання додаткової інформації див [підключення служби Office 365 групи, за допомогою ineterface користувача SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="bf718-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="bf718-113">Створити Office 365 Група пов'язаних сайт, потрібно буде створити сайт групи.</span><span class="sxs-lookup"><span data-stu-id="bf718-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="bf718-114">Для отримання додаткової інформації дивіться [Створення сайту групи в SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="bf718-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

