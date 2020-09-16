---
title: Обмеження доступу в SharePoint або OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: d8be1eb5bdcd0b5b08ddad32a45b6282c788c26a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720703"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="e982d-102">Обмеження доступу в SharePoint або OneDrive</span><span class="sxs-lookup"><span data-stu-id="e982d-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="e982d-103">У SharePoint і OneDrive обмежити доступ до елементів, як-от файли, папки та списки, надавши доступ лише групам або особам, до яких потрібно мати доступ.</span><span class="sxs-lookup"><span data-stu-id="e982d-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="e982d-104">За замовчуванням дозволи в SharePoint успадковуються від більшого в ієрархії.</span><span class="sxs-lookup"><span data-stu-id="e982d-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="e982d-105">Таким чином, файл успадковує свої дозволи з папки, які успадковують свої дозволи від бібліотеки, що успадковує її дозволи від сайту.</span><span class="sxs-lookup"><span data-stu-id="e982d-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="e982d-106">Ви можете надати спільний доступ на вищому рівні (наприклад, надавати спільний доступ до всього сайту), а потім розірвати успадкування, якщо ви не хочете надавати спільний доступ до всіх елементів на сайті.</span><span class="sxs-lookup"><span data-stu-id="e982d-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="e982d-107">Але ми не радимо це робити, тому що він робить збереження дозволів складнішими та заплутаною в майбутньому.</span><span class="sxs-lookup"><span data-stu-id="e982d-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="e982d-108">Ось що можна зробити, а потім:</span><span class="sxs-lookup"><span data-stu-id="e982d-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="e982d-109">Якщо, наприклад, потрібно надати спільний доступ до всього вмісту папки, окрім одного файлу, перетягніть цей файл до нового розташування, який не надано спільний доступ.</span><span class="sxs-lookup"><span data-stu-id="e982d-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="e982d-110">Якщо в папці є дві вкладені папки, і потрібно надати спільний доступ до однієї вкладеної папки за допомогою груп A і B, а також дозволити лише групі доступу до другої вкладеної папки, надати спільний доступ до батьківської теки за допомогою групи A і додати групу B до першої вкладеної підпапки.</span><span class="sxs-lookup"><span data-stu-id="e982d-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="e982d-111">Скасування спільного доступу до файлу або папки </span><span class="sxs-lookup"><span data-stu-id="e982d-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

