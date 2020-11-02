---
title: Помилка 0x8004de40 під час запуску OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823122"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="10f60-102">Помилка 0x8004de40 під час запуску OneDrive</span><span class="sxs-lookup"><span data-stu-id="10f60-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="10f60-103">Якщо під час входу в службу OneDrive з'являється повідомлення про помилку **0x8004de40** , перезавантажте комп'ютер під час підключення до робочого або навчального домену.</span><span class="sxs-lookup"><span data-stu-id="10f60-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="10f60-104">Якщо ви отримали цю помилку після перезавантаження, випробуйте цей час, коли підключаєтеся до робочого або навчального домену, виконайте такі дії:</span><span class="sxs-lookup"><span data-stu-id="10f60-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="10f60-105">Натисніть кнопку Пуск і введіть **CMD** або **командний рядок**  у полі пошуку, клацніть правою кнопкою миші у програмі командний рядок і виберіть команду  **Запуск із правами адміністратора** .</span><span class="sxs-lookup"><span data-stu-id="10f60-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator** .</span></span> <span data-ttu-id="10f60-106">Якщо з'явиться запит на введення пароля адміністратора або підтвердження, введіть пароль або натисніть кнопку **дозволити** .</span><span class="sxs-lookup"><span data-stu-id="10f60-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow** .</span></span>  

2. <span data-ttu-id="10f60-107">У вікні командного рядка введіть **dsregcmd/Leave**  і зачекайте, доки команда завершиться.</span><span class="sxs-lookup"><span data-stu-id="10f60-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="10f60-108">Потім введіть **dsregcmd/JOIN** і зачекайте, доки команда завершиться.</span><span class="sxs-lookup"><span data-stu-id="10f60-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="10f60-109">Перезавантажте комп'ютер.</span><span class="sxs-lookup"><span data-stu-id="10f60-109">Reboot your computer.</span></span>
