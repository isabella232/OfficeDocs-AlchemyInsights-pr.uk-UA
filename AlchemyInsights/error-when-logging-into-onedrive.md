---
title: 0x8004de40 під час запуску OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813673"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="c0f83-102">0x8004de40 під час запуску OneDrive</span><span class="sxs-lookup"><span data-stu-id="c0f83-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="c0f83-103">Якщо під час входу **у OneDrive 0x8004de40** з'являється повідомлення про помилку, перезавантажте комп'ютер під час підключення до робочого або навчального домену.</span><span class="sxs-lookup"><span data-stu-id="c0f83-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="c0f83-104">Якщо після перезавантаження з'являється таке повідомлення про помилку, спробуйте таке під час підключення до робочого або навчального домену:</span><span class="sxs-lookup"><span data-stu-id="c0f83-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="c0f83-105">Натисніть кнопку Пуск і введіть **cmd** або **командний** рядок у полі пошуку, клацніть правою кнопкою миші програму командного рядка та виберіть **команду Запустити з правами адміністратора.**</span><span class="sxs-lookup"><span data-stu-id="c0f83-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator**.</span></span> <span data-ttu-id="c0f83-106">Якщо буде запропоновано ввести пароль адміністратора або підтвердження, введіть пароль або натисніть кнопку **Дозволити.**</span><span class="sxs-lookup"><span data-stu-id="c0f83-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow**.</span></span>  

2. <span data-ttu-id="c0f83-107">У вікні Командний рядок введіть **dsregcmd /leave**  і зачекайте, доки не завершиться команда.</span><span class="sxs-lookup"><span data-stu-id="c0f83-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="c0f83-108">Потім введіть **dsregcmd /join і** дочекайтеся завершення команди.</span><span class="sxs-lookup"><span data-stu-id="c0f83-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="c0f83-109">Перезавантажте комп'ютер.</span><span class="sxs-lookup"><span data-stu-id="c0f83-109">Reboot your computer.</span></span>
