---
title: Настроювання виключень для сканування АТФ у програмі Microsoft Defender
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
ms.openlocfilehash: 912e77b9b1a149fef373f2d0814fb2f0671a48c6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "50714356"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="05357-102">Настроювання виключень для сканування АТФ у програмі Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="05357-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="05357-103">Загалом можна виключити певні розширення файлів і розташування папок із сканувань АТФ в програмі Microsoft Defender.</span><span class="sxs-lookup"><span data-stu-id="05357-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="05357-104">Крім того, можна настроїти винятки для файлів, які відкриваються певними процесами.</span><span class="sxs-lookup"><span data-stu-id="05357-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="05357-105">Докладні відомості наведено в статті, [Настроювання та перевірка виключень на основі розширення файлу та розташування папки](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) та [Настроювання виключень для файлів, які відкриваються процесами](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span><span class="sxs-lookup"><span data-stu-id="05357-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="05357-106">Щоб настроїти винятки для  **Windows server 2016 і 2019**, ознайомтеся [з настроюванням антивірусних програм Microsoft Defender на сервері Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="05357-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="05357-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="05357-107">**Mac**</span></span>

<span data-ttu-id="05357-108">Докладні відомості про підтримувані типи виключень і настроювання списку винятків для Mac наведено в статті [Підтримувані типи виключень](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) і [Настроювання списку виключень](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span><span class="sxs-lookup"><span data-stu-id="05357-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="05357-109">**Примітка** . Крім того, можна перевірити списки виключень, використовуючи тестовий файл EICAR.</span><span class="sxs-lookup"><span data-stu-id="05357-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="05357-110">Докладні відомості наведено в статті перевірка [виключень списків із тестовими файлами EICAR](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="05357-110">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="05357-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="05357-111">**Linux**</span></span>

<span data-ttu-id="05357-112">Докладні відомості про підтримувані типи виключень і налаштування списку винятків для Linux наведено в статті [Підтримувані типи виключень](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) і [Настроювання та перевірка виключень для системи Microsoft Defender для Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span><span class="sxs-lookup"><span data-stu-id="05357-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="05357-113">**Примітка** . Крім того, можна перевірити списки виключень, використовуючи тестовий файл EICAR.</span><span class="sxs-lookup"><span data-stu-id="05357-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="05357-114">Докладні відомості наведено в статті перевірка [виключень списків із тестовими файлами EICAR](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="05357-114">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 