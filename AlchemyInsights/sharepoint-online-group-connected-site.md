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
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="2069d-102">Проблеми під час створення групи підключених сайтів у SharePoint</span><span class="sxs-lookup"><span data-stu-id="2069d-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="2069d-103">Деякі поширені проблеми виникають під час створення або повторного створення підключеного сайту групи.</span><span class="sxs-lookup"><span data-stu-id="2069d-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="2069d-104">Якщо ви видалили групу та його підключений сайт і хочете створити інший сайт з тією самою URL-адресою, потрібно остаточно видалити попередній сайт.</span><span class="sxs-lookup"><span data-stu-id="2069d-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="2069d-105">Завантажити [оболонку керування](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429) в "спо"</span><span class="sxs-lookup"><span data-stu-id="2069d-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="2069d-106">Докладні відомості про початок роботи з PowerShell наведено в статті [початок роботи з оболонкою керування службою SharePoint Online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="2069d-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="2069d-107">Видаліть сайт із видалених сайтів за допомогою командлета [Remove-Spodeableedsite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell.</span><span class="sxs-lookup"><span data-stu-id="2069d-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="2069d-108">PowerShell потрібен для остаточного видалення сайтів групи.</span><span class="sxs-lookup"><span data-stu-id="2069d-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="2069d-109">Якщо ви створюєте сайт, підключений до групи, і отримаєте попередження: **інша група з тим самим псевдонімом уже існує**, перевірте наявні групи в [центрі адміністрування Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="2069d-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="2069d-110">Щоб вирішити цю проблему, видаліть наявну групу, якщо вона більше не потрібна, або створіть сайт з іншим призначенням псевдоніма.</span><span class="sxs-lookup"><span data-stu-id="2069d-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="2069d-111">Існує кілька способів створення та використання сучасних груп у службі SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2069d-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="2069d-112">До групи Microsoft 365 можна підключити вже доступні сайти.</span><span class="sxs-lookup"><span data-stu-id="2069d-112">You can connect existing sites to a Microsoft 365 group.</span></span> <span data-ttu-id="2069d-113">Докладні відомості наведено в статті [підключення групи Microsoft 365 за допомогою інтерфейсу користувача SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="2069d-113">For more info, see [Connect a Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="2069d-114">Щоб створити сайт, підключений до групи Microsoft 365, потрібно створити [сайт групи](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="2069d-114">To create a Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
