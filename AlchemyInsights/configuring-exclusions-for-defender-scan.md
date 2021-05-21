---
title: Налаштування винятків для перевірки РВЗ для Microsoft Defender
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
- "6027"
- "9001464"
ms.openlocfilehash: 5eb18f4133aca93c1506f4975c8d0567bede8d57
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543706"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="ca966-102">Налаштування винятків для перевірки РВЗ для Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="ca966-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="ca966-103">Загалом із АТС Microsoft Defender можна виключити певні розширення файлів і розташування папок.</span><span class="sxs-lookup"><span data-stu-id="ca966-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="ca966-104">Ви також можете налаштувати винятки для файлів, відкритих у певних процесах.</span><span class="sxs-lookup"><span data-stu-id="ca966-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="ca966-105">Докладні відомості див. в розділах Настроювання та перевірка винятків на основі розширення та розташування папки та Налаштування винятків для файлів, відкритих [процесами.](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) [](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="ca966-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="ca966-106">Відомості про налаштування винятків для **Windows Server 2016 і 2019** див. в Антивірус для Microsoft Defender на Windows [Server.](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="ca966-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="ca966-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="ca966-107">**Mac**</span></span>

<span data-ttu-id="ca966-108">Докладні відомості про підтримувані типи винятків і налаштування списку [](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) винятків для Mac див. в статтях Підтримувані типи винятків і Налаштування списку [винятків.](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions)</span><span class="sxs-lookup"><span data-stu-id="ca966-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="ca966-109">**Примітка** Ви також можете перевірити списки винятків, використовуючи тестовий файл EICAR.</span><span class="sxs-lookup"><span data-stu-id="ca966-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="ca966-110">Докладні відомості див. в сторінці Перевірка списків винятків [за допомогою тестової файлу EICAR.](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="ca966-110">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="ca966-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="ca966-111">**Linux**</span></span>

<span data-ttu-id="ca966-112">Докладні відомості про підтримувані типи винятків і налаштування списку [](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) винятків для Linux див. в розділах Підтримувані типи винятків і Налаштування та перевірка винятків для АТФ для [Microsoft Defender для Linux.](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions)</span><span class="sxs-lookup"><span data-stu-id="ca966-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="ca966-113">**Примітка** Ви також можете перевірити списки винятків, використовуючи тестовий файл EICAR.</span><span class="sxs-lookup"><span data-stu-id="ca966-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="ca966-114">Докладні відомості див. в сторінці Перевірка списків винятків [за допомогою тестової файлу EICAR.](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="ca966-114">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 