---
title: Засіб діагностики служби для віртуального робочого стола Windows
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
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/05/2021
ms.locfileid: "51596043"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="88a11-102">Засіб діагностики служби для віртуального робочого стола Windows</span><span class="sxs-lookup"><span data-stu-id="88a11-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="88a11-103">Віртуальний робочий стіл Windows (WVD) пропонує засіб діагностики, який дає змогу адміністраторам визначити помилки в одному інтерфейсі.</span><span class="sxs-lookup"><span data-stu-id="88a11-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="88a11-104">Цей засіб реєструє діагностичні відомості щоразу, коли WVD використовується користувачем, який призначає роль WVD.</span><span class="sxs-lookup"><span data-stu-id="88a11-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="88a11-105">Кожен журнал містить відомості про роль WVD, залучену до дії, повідомлення про помилку, які відображаються під час сеансу, а також відомості про клієнта та користувача.</span><span class="sxs-lookup"><span data-stu-id="88a11-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="88a11-106">Аналітика журналів Azure можна налаштувати на записування журналу дій, створеного засобом діагностики, виконавши такі дії:</span><span class="sxs-lookup"><span data-stu-id="88a11-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool by following these steps:</span></span>

1. <span data-ttu-id="88a11-107">Створіть робочу область Log Analytics за допомогою [порталу Azure](https://go.microsoft.com/fwlink/?linkid=2129500) або [Azure PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)</span><span class="sxs-lookup"><span data-stu-id="88a11-107">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>

1. <span data-ttu-id="88a11-108">[Підключіть комп'ютери з Windows до монітора Azure](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="88a11-108">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="88a11-109">Отримайте ідентифікатор робочої області та первинний ключ робочої області.</span><span class="sxs-lookup"><span data-stu-id="88a11-109">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="88a11-110">Ці відомості необхідно налаштувати в майстрі налаштування для належного налаштування агента та забезпечення його зв'язку з монітором Azure.</span><span class="sxs-lookup"><span data-stu-id="88a11-110">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>

1. <span data-ttu-id="88a11-111">[Push-дані діагностики до робочої області.](https://go.microsoft.com/fwlink/?linkid=2128284)</span><span class="sxs-lookup"><span data-stu-id="88a11-111">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="88a11-112">Ви можете переносити діагностичні дані з клієнта WVD до аналітики журналів для робочої області.</span><span class="sxs-lookup"><span data-stu-id="88a11-112">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>

1. <span data-ttu-id="88a11-113">[Визначте та діагностувати](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) проблеми, які є внутрішніми або зовнішніми у зв'язанні із WVD.</span><span class="sxs-lookup"><span data-stu-id="88a11-113">[Identify and diagnose](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) issues that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="88a11-114">Докладні відомості про настроювання засобу діагностики служби для WVD див. в статтях Використання аналітики журналу для функції діагностики.</span><span class="sxs-lookup"><span data-stu-id="88a11-114">To learn more about configuring the service diagnostics tool for WVD, see Use Log Analytics for the diagnostics feature.</span></span>