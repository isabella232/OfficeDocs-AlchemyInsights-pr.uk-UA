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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/18/2019
ms.locfileid: "36551472"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="f6aaa-102">Обмеження доступу в SharePoint або OneDrive</span><span class="sxs-lookup"><span data-stu-id="f6aaa-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="f6aaa-103">У SharePoint і OneDrive ви Обмежте доступ до таких елементів, як файли, папки та списки, надаючи доступ лише до груп або осіб, яким потрібно мати доступ.</span><span class="sxs-lookup"><span data-stu-id="f6aaa-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="f6aaa-104">За промовчанням дозволи в SharePoint успадковуються від вище в ієрархії.</span><span class="sxs-lookup"><span data-stu-id="f6aaa-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="f6aaa-105">Таким чином, файл успадковує свої дозволи з папки, яка успадковує свої дозволи від бібліотеки, яка успадковує свої дозволи від сайту.</span><span class="sxs-lookup"><span data-stu-id="f6aaa-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="f6aaa-106">Ви можете обмінюватися на вищому рівні (наприклад, розділяючи весь сайт), а потім розірвати успадкування, якщо ви не хочете ділитися всіма об'єктами на сайті.</span><span class="sxs-lookup"><span data-stu-id="f6aaa-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="f6aaa-107">Однак, ми не рекомендуємо це, тому що це робить підтримання дозволів більш складним і заплутаним в майбутньому.</span><span class="sxs-lookup"><span data-stu-id="f6aaa-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="f6aaa-108">Ось що ви могли б зробити замість цього:</span><span class="sxs-lookup"><span data-stu-id="f6aaa-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="f6aaa-109">Якщо, наприклад, потрібно надати спільний доступ до вмісту папки, за винятком одного файлу в ньому, перемістіть цей файл до нового розташування, який не є спільним.</span><span class="sxs-lookup"><span data-stu-id="f6aaa-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="f6aaa-110">Якщо у папці є дві вкладені папки, і потрібно надати спільний доступ до однієї вкладеної папки з групами A та B, а також дозволити лише групувати до другої вкладеної папки, поділіться батьківською папкою з групою A і додайте групу B до першої вкладеної теки.</span><span class="sxs-lookup"><span data-stu-id="f6aaa-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="f6aaa-111">Припинення спільного доступу до файлу або папки</span><span class="sxs-lookup"><span data-stu-id="f6aaa-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

