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
ms.openlocfilehash: 14ad9dd094902c85eaf0398c76003cea20ad4c0a
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051122"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="2e22b-102">Проблеми під час створення або групи підключених сайтів у SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="2e22b-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="2e22b-103">Існує кілька поширених проблем, які виникають під час створення або Повторне створення групи, підключеного сайту.</span><span class="sxs-lookup"><span data-stu-id="2e22b-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="2e22b-104">Якщо ви видалили групу та її підключений сайт і бажаєте створити інший сайт з однаковою URL-адресою, потрібно остаточно видалити попередній сайт.</span><span class="sxs-lookup"><span data-stu-id="2e22b-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="2e22b-105">Завантажити [оболонку керування спо](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="2e22b-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="2e22b-106">Щоб отримати додаткові відомості про початок роботи з PowerShell, див. [початок роботи з оболонки керування SharePoint Online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="2e22b-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="2e22b-107">Видалення сайту з видалених сайтів за допомогою командлета [видалення-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell.</span><span class="sxs-lookup"><span data-stu-id="2e22b-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="2e22b-108">Якщо ви створюєте сайт групи, підключений і отримати попередження іншу групу з таким самим псевдонімом вже існує, перевірте наявні групи з [Office 365 з центру адміністрування](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="2e22b-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="2e22b-109">Щоб вирішити цю проблему, видаліть наявну групу, якщо вона більше не потрібна, або створіть сайт з іншим псевдонімом.</span><span class="sxs-lookup"><span data-stu-id="2e22b-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="2e22b-110">Існують різні способи створення та використання сучасних груп з SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2e22b-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="2e22b-111">Можна підключити наявні сайти до групи Office 365.</span><span class="sxs-lookup"><span data-stu-id="2e22b-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="2e22b-112">Для отримання додаткових відомостей див. [підключення групи Office 365 за допомогою користувача SharePoint ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="2e22b-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="2e22b-113">Щоб створити групу Office 365, підключений сайт, потрібно створити сайт групи.</span><span class="sxs-lookup"><span data-stu-id="2e22b-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="2e22b-114">Для отримання додаткових відомостей див. [Створення сайту групи в SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="2e22b-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

