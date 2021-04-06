---
title: Визначення проблем із віртуальним робочим столом Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/05/2021
ms.locfileid: "51596038"
---
# <a name="identify-windows-virtual-desktop-issues"></a><span data-ttu-id="4f638-102">Визначення проблем із віртуальним робочим столом Windows</span><span class="sxs-lookup"><span data-stu-id="4f638-102">Identify Windows Virtual Desktop issues</span></span>

<span data-ttu-id="4f638-103">У службі діагностики віртуальних робочих столів Windows використовується лише один командлет PowerShell, але містить багато необов'язкових параметрів, щоб усунути й усунути проблеми.</span><span class="sxs-lookup"><span data-stu-id="4f638-103">Windows Virtual Desktop Diagnostics uses just one PowerShell cmdlet but contains many optional parameters to help narrow down and isolate issues.</span></span> <span data-ttu-id="4f638-104">Початок роботи</span><span class="sxs-lookup"><span data-stu-id="4f638-104">To get started:</span></span> 

1. <span data-ttu-id="4f638-105">Завантажте та імпортуйте модуль PowerShell для Windows Virtual Desktop.</span><span class="sxs-lookup"><span data-stu-id="4f638-105">Download and import the Windows Virtual Desktop PowerShell module.</span></span> <span data-ttu-id="4f638-106">Докладні відомості див. в [командлетах Windows Virtual Desktop для Windows PowerShell.](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)</span><span class="sxs-lookup"><span data-stu-id="4f638-106">For details, see [Windows Virtual Desktop Cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span></span>

1. <span data-ttu-id="4f638-107">Щоб увійти у свій обліковий запис, запустіть цей командлет:</span><span class="sxs-lookup"><span data-stu-id="4f638-107">Run the following cmdlet to sign in to your account:</span></span>
    
    <span data-ttu-id="4f638-108">Приклад: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span><span class="sxs-lookup"><span data-stu-id="4f638-108">Example: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span></span>

<span data-ttu-id="4f638-109">**ПРИМІТКА.** Усі запити, які використовують PowerShell, мають містити параметри -UserName або -ActivityID.</span><span class="sxs-lookup"><span data-stu-id="4f638-109">**NOTE:** All queries using PowerShell must include either the -UserName or -ActivityID parameters.</span></span> <span data-ttu-id="4f638-110">Відомості про можливості моніторингу див. в відомості про використання аналітики журналів для [функції діагностики.](https://go.microsoft.com/fwlink/?linkid=2126847)</span><span class="sxs-lookup"><span data-stu-id="4f638-110">For monitoring capabilities, see Use [Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2126847).</span></span>

<span data-ttu-id="4f638-111">Щоб відфільтрувати дії діагностики за користувачем, запустіть такий командлет:</span><span class="sxs-lookup"><span data-stu-id="4f638-111">To filter diagnostic activities by user, run the following cmdlet:</span></span>

<span data-ttu-id="4f638-112">Приклад: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span><span class="sxs-lookup"><span data-stu-id="4f638-112">Example: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span></span>

<span data-ttu-id="4f638-113">Щоб виявити проблеми, можна запустити список фільтрів.</span><span class="sxs-lookup"><span data-stu-id="4f638-113">There is a list of filters you can run to diagnose issues.</span></span> <span data-ttu-id="4f638-114">Докладні відомості про діагностування неполадок див. в статтях [Визначення та діагностування проблем із віртуальним робочим столом Windows.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)</span><span class="sxs-lookup"><span data-stu-id="4f638-114">To learn more about diagnosing issues, see [Identify and diagnose Windows Virtual Desktop issues](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span></span>

<span data-ttu-id="4f638-115">Докладні відомості про поширені помилки див. в [статтях Загальні помилки senarios.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios)</span><span class="sxs-lookup"><span data-stu-id="4f638-115">To learn more about common errors, see [Common errors senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span></span>
