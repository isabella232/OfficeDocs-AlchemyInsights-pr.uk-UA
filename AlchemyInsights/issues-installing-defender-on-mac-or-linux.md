---
title: Проблеми з інсталяцією Microsoft Defender на комп'ютері Mac або Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: a8d5ad2246b9b83e1e0a4d5be4dd8bb41c16e734
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "50714320"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a><span data-ttu-id="f621d-102">Проблеми з інсталяцією Microsoft Defender на комп'ютері Mac або Linux</span><span class="sxs-lookup"><span data-stu-id="f621d-102">Issues installing Microsoft Defender on Mac or Linux</span></span>

<span data-ttu-id="f621d-103">**Mac**</span><span class="sxs-lookup"><span data-stu-id="f621d-103">**Mac**</span></span>

- <span data-ttu-id="f621d-104">Переконайтеся, що Системні вимоги виконуються, перш ніж інсталювати програму Microsoft Defender АТФ для Mac.</span><span class="sxs-lookup"><span data-stu-id="f621d-104">Ensure that system requirements are met before installing Microsoft Defender ATP for Mac.</span></span> <span data-ttu-id="f621d-105">Щоб отримати докладні відомості, Дізнайтеся, [як інсталювати програму Microsoft DEFENDER АТФ для Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span><span class="sxs-lookup"><span data-stu-id="f621d-105">For more info, see [How to install Microsoft Defender ATP for Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span></span>  
- <span data-ttu-id="f621d-106">Перегляньте інформацію у файлі: "/Library/Logs/Microsoft/mdatp/install.log".</span><span class="sxs-lookup"><span data-stu-id="f621d-106">Review the information in the file: "/Library/Logs/Microsoft/mdatp/install.log".</span></span>

<span data-ttu-id="f621d-107">**Linux**</span><span class="sxs-lookup"><span data-stu-id="f621d-107">**Linux**</span></span>

- <span data-ttu-id="f621d-108">Переконайтеся, що Системні вимоги виконуються, перш ніж інсталювати програму Microsoft Defender АТФ для Linux.</span><span class="sxs-lookup"><span data-stu-id="f621d-108">Ensure that system requirements are met before installing Microsoft Defender ATP for Linux.</span></span> <span data-ttu-id="f621d-109">Щоб отримати докладні відомості, Дізнайтеся, [як інсталювати програму Microsoft DEFENDER АТФ для Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span><span class="sxs-lookup"><span data-stu-id="f621d-109">For more info, see [How to install Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span> 
- <span data-ttu-id="f621d-110">Щоб перевірити, чи запущено службу MDATP, перегляньте статтю [Помилка інсталяції](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span><span class="sxs-lookup"><span data-stu-id="f621d-110">To verify that MDATP service is running, see [Installation failed](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span></span>  
    <span data-ttu-id="f621d-111">Щоб усунути неполадки та вирішити проблеми, якщо служба не запущена, перегляньте [кроки з усунення несправностей, якщо служба mdatp не запущена](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span><span class="sxs-lookup"><span data-stu-id="f621d-111">To troubleshoot and resolve issues if the service is not running, see [Steps to troubleshoot if mdatp service isn't running](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span></span>
- <span data-ttu-id="f621d-112">Щоб перевірити конфігурацію клієнта, у якому перевіряється стан справності продукту, а також для запуску тесту виявлення в текстовому файлі EICAR, перегляньте статтю [Конфігурація клієнта](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span><span class="sxs-lookup"><span data-stu-id="f621d-112">For steps to check the client configuration, which verifies the health of the product, and to run a detection test on the EICAR text file, see [Client configuration](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span></span>  

    <span data-ttu-id="f621d-113">**Примітка** . Щоб переглянути список підтримуваних файлових систем для роботи з доступом, ознайомтеся з [програмою Microsoft DEFENDER АТФ для Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span><span class="sxs-lookup"><span data-stu-id="f621d-113">**Note** For a list of supported file systems for on-access activity, see [Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span>