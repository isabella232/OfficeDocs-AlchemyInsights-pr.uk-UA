---
title: Обмеження доступу в SharePoint або OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e5458226fe33bd5cb3da1f608fb113b888fbfd16
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551472"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="f3491-102">Обмеження доступу в SharePoint або OneDrive</span><span class="sxs-lookup"><span data-stu-id="f3491-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="f3491-103">У SharePoint і OneDrive Вам обмежити доступ до пунктам, як файли, папки та списки надавши права доступу лише для особи або групи осіб, які ви хочете мати доступ.</span><span class="sxs-lookup"><span data-stu-id="f3491-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="f3491-104">За промовчанням дозволи в SharePoint успадковано від вище вгору в ієрархії.</span><span class="sxs-lookup"><span data-stu-id="f3491-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="f3491-105">Так файл успадковують його дозволи з папки, які успадковують його дозволи з бібліотеки, які успадковують його дозволи від сайту.</span><span class="sxs-lookup"><span data-stu-id="f3491-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="f3491-106">Ви можете поділитися на вищому рівні (таких як шляхом обміну всього сайту) і потім розбити спадкування, якщо ви не хочете ділитися всі предмети на сайті.</span><span class="sxs-lookup"><span data-stu-id="f3491-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="f3491-107">Однак, не рекомендується це тому, що це робить підтримання дозволи більш складною і заплутаною в майбутньому.</span><span class="sxs-lookup"><span data-stu-id="f3491-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="f3491-108">Ось те, що ви могли б зробити замість цього:</span><span class="sxs-lookup"><span data-stu-id="f3491-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="f3491-109">Якщо, наприклад, ви хочете поділитися весь вміст папки, за винятком одного файлу в ньому, перемістити цей файл до нового розташування, які не є спільним.</span><span class="sxs-lookup"><span data-stu-id="f3491-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="f3491-110">Якщо у вас є два вкладені папки в папці, і ви хочете, щоб поділитися один вкладену папку з групи A та B і дозволити тільки Група A доступ до другого підпапку, поділитися батьківську папку з групи A та додати Група B першу вкладену папку.</span><span class="sxs-lookup"><span data-stu-id="f3491-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="f3491-111">Закрити спільний доступ до файлу або папки</span><span class="sxs-lookup"><span data-stu-id="f3491-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

