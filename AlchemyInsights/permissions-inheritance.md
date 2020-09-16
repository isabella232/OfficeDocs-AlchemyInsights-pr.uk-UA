---
title: Успадкування дозволів
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bb5c440a-ca70-4dc6-b517-688e80551101
ms.openlocfilehash: f086bd7312772b399146cd81261f147364d64665
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741972"
---
# <a name="how-permissions-inheritance-works-in-sharepoint"></a><span data-ttu-id="a2bb4-102">Принцип роботи успадкування дозволів у SharePoint</span><span class="sxs-lookup"><span data-stu-id="a2bb4-102">How permissions inheritance works in SharePoint</span></span>

<span data-ttu-id="a2bb4-103">За замовчуванням дозволи в SharePoint успадковуються від більшого в ієрархії.</span><span class="sxs-lookup"><span data-stu-id="a2bb4-103">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="a2bb4-104">Таким чином, файл успадковує свої дозволи з папки, які успадковують свої дозволи від бібліотеки, які успадковують свої дозволи від сайту, що успадковує її дозволи від колекції сайтів.</span><span class="sxs-lookup"><span data-stu-id="a2bb4-104">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site, which inherits its permissions from the site collection.</span></span>
  
<span data-ttu-id="a2bb4-105">Докладні відомості про видалення унікальних дозволів і відновлення успадкування наведено в статті [редагування та керування дозволами для списку або бібліотеки](https://go.microsoft.com/fwlink/?linkid=869946).</span><span class="sxs-lookup"><span data-stu-id="a2bb4-105">For info about removing unique permissions and restoring inheritance, see [Edit and manage permissions for a list or library](https://go.microsoft.com/fwlink/?linkid=869946).</span></span>
  

