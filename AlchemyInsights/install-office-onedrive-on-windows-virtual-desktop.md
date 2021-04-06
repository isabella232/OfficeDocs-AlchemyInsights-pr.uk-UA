---
title: Інсталяція Office і OneDrive на віртуальному робочому столі Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: fb38f46cced928e33e16e8e83ad740dd83aea622
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/05/2021
ms.locfileid: "51596029"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a><span data-ttu-id="603e9-102">Інсталяція Office і OneDrive на віртуальному робочому столі Windows</span><span class="sxs-lookup"><span data-stu-id="603e9-102">Install Office and OneDrive on Windows Virtual Desktop</span></span>

1. <span data-ttu-id="603e9-103">[Підготуйте та налаштуйте зразок зображення VHD](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image).</span><span class="sxs-lookup"><span data-stu-id="603e9-103">[Prepare and customize a master VHD image](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image).</span></span> <span data-ttu-id="603e9-104">Створіть віртуальну машину (VM), якщо її ще не створено.</span><span class="sxs-lookup"><span data-stu-id="603e9-104">Create a virtual machine (VM) if it hasn't already been created.</span></span>

1. <span data-ttu-id="603e9-105">[Інсталюйте пакет Office у режимі активації на спільному комп'ютері.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode)</span><span class="sxs-lookup"><span data-stu-id="603e9-105">[Install Office in shared computer activation mode](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode).</span></span> <span data-ttu-id="603e9-106">Активація на спільному комп'ютері дає змогу кільком користувачам отримувати доступ до Office.</span><span class="sxs-lookup"><span data-stu-id="603e9-106">Shared computer activation allows multiple users to access Office.</span></span>

1. <span data-ttu-id="603e9-107">[Інсталюйте OneDrive у режимі на комп'ютері.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode)</span><span class="sxs-lookup"><span data-stu-id="603e9-107">[Install OneDrive in per-machine mode](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode).</span></span> <span data-ttu-id="603e9-108">Зазвичай програму OneDrive інстальовано для кожного користувача, але тут її потрібно інсталювати на комп'ютер.</span><span class="sxs-lookup"><span data-stu-id="603e9-108">Normally, OneDrive is installed per user, but here, it should be installed per machine.</span></span>