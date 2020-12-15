---
title: Засіб діагностики служби для віртуального настільного комп'ютера Windows
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/14/2020
ms.locfileid: "49680236"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="9cb41-102">Засіб діагностики служби для віртуального настільного комп'ютера Windows</span><span class="sxs-lookup"><span data-stu-id="9cb41-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="9cb41-103">Віртуальна стільниця Windows (WVD) пропонує засіб діагностики, який дає змогу адміністраторам визначати помилки за допомогою одного інтерфейсу.</span><span class="sxs-lookup"><span data-stu-id="9cb41-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="9cb41-104">Цей засіб реєструє дані, пов'язані з діагностикою, коли хтось використовує роль WVD.</span><span class="sxs-lookup"><span data-stu-id="9cb41-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="9cb41-105">Кожен журнал містить відомості про роль WVD, яка бере участь у цій діяльності, повідомлення про помилки, які відображаються під час сеансу, а також відомості про клієнта та користувача.</span><span class="sxs-lookup"><span data-stu-id="9cb41-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="9cb41-106">Для захоплення журналу дій, створеного діагностичним засобом, можна налаштувати Журнал активності.</span><span class="sxs-lookup"><span data-stu-id="9cb41-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool.</span></span> <span data-ttu-id="9cb41-107">Ось як це зробити.</span><span class="sxs-lookup"><span data-stu-id="9cb41-107">Here's how:</span></span>

1. <span data-ttu-id="9cb41-108">Створіть робочу область аналітики журналів з [лазуропорталом](https://go.microsoft.com/fwlink/?linkid=2129500) або [лазуровий PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span><span class="sxs-lookup"><span data-stu-id="9cb41-108">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>
1. <span data-ttu-id="9cb41-109">[Підключіть комп'ютери з ОС Windows до Лазурого монітора](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="9cb41-109">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="9cb41-110">Отримання ІДЕНТИФІКАТОРА робочої області та первинного ключа робочої області.</span><span class="sxs-lookup"><span data-stu-id="9cb41-110">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="9cb41-111">Майстер настроювання має надати цю інформацію належним чином настроїти агент і переконатися, що він може спілкуватися з лазуровий монітор.</span><span class="sxs-lookup"><span data-stu-id="9cb41-111">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>
1. <span data-ttu-id="9cb41-112">[Push-діагностика даних в робочій області](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="9cb41-112">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="9cb41-113">Ви можете Push-дані діагностики з клієнта WVD для журналу аналітики для своєї робочої області.</span><span class="sxs-lookup"><span data-stu-id="9cb41-113">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>
1. <span data-ttu-id="9cb41-114">[Виявлення та діагностика проблем](https://go.microsoft.com/fwlink/?linkid=2128338) , які є внутрішніми або зовнішніми відносно wvd.</span><span class="sxs-lookup"><span data-stu-id="9cb41-114">[Identify and diagnose issues](https://go.microsoft.com/fwlink/?linkid=2128338) that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="9cb41-115">Щоб дізнатися більше про те, як настроїти засіб діагностики служби для WVD, перегляньте статтю [використання журналу Analytics для функції діагностики](https://go.microsoft.com/fwlink/?linkid=2128084).</span><span class="sxs-lookup"><span data-stu-id="9cb41-115">To learn more about configuring the service diagnostics tool for WVD, see [Use Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2128084).</span></span>
