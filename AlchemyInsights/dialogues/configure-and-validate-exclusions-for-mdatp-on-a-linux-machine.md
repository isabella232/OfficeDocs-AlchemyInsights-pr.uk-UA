---
title: Настроювання та перевірка виключень для MDATP на комп'ютері Linux
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696074"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a><span data-ttu-id="f3fcb-102">Настроювання та перевірка виключень для MDATP на комп'ютері Linux</span><span class="sxs-lookup"><span data-stu-id="f3fcb-102">Configure and validate exclusions for MDATP on a Linux machine</span></span>

<span data-ttu-id="f3fcb-103">Ви можете виключити певні файли, папки, процеси та файли, відкриті в процесі перевірки MDATP.</span><span class="sxs-lookup"><span data-stu-id="f3fcb-103">You can exclude certain files, folders, processes, and process-opened files from MDATP scans.</span></span> <span data-ttu-id="f3fcb-104">Винятки допомагають запобігти неправильному виявленню програмного забезпечення та файлів, які унікальні або настроєні для вашої організації.</span><span class="sxs-lookup"><span data-stu-id="f3fcb-104">Exclusions help prevent incorrect detection of software and files unique or customized to your organization.</span></span> <span data-ttu-id="f3fcb-105">Винятки також допомагають зменшити неполадки продуктивності, викликані MDATP.</span><span class="sxs-lookup"><span data-stu-id="f3fcb-105">Exclusions also help mitigate performance problems caused by MDATP.</span></span>

<span data-ttu-id="f3fcb-106">Докладні відомості наведено в статті [Настроювання та перевірка винятків для MDATP для Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span><span class="sxs-lookup"><span data-stu-id="f3fcb-106">To learn more, see [Configure and validate exclusions for MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="f3fcb-107">Винятки, описані в цій статті, не застосовуватимуться до інших можливостей MDATP для Linux, зокрема виявлення кінцевих точок і відповіді (пед).</span><span class="sxs-lookup"><span data-stu-id="f3fcb-107">The exclusions described in this article don't apply to other capabilities of MDATP for Linux, including endpoint detection and response (EDR).</span></span> <span data-ttu-id="f3fcb-108">Файли, які ви виключаєте, використовуючи методи, описані в цій статті, можуть ініціювати оповіщення EDR та інші можливості виявлення.</span><span class="sxs-lookup"><span data-stu-id="f3fcb-108">Files that you exclude by using the methods described in this article can still trigger EDR alerts and other detection capabilities.</span></span>
