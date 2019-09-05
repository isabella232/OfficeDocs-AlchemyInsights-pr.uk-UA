---
title: Інсталяція Office на сервері терміналів-ліцензовано
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 53071224a7c33532d864cd70b84bf0e3cc6a992f
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36735410"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="1411b-102">Інсталяція Office на сервері терміналів</span><span class="sxs-lookup"><span data-stu-id="1411b-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="1411b-103">Для розгортання Office 365 ProPlus на сервері Windows за допомогою служб віддалених робочих столів (RDS), раніше іменований служби терміналів:</span><span class="sxs-lookup"><span data-stu-id="1411b-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="1411b-104">Потрібно мати Office 365 план, який включає в себе Office 365 ProPlus, наприклад Office 365 Enterprise E3 або Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="1411b-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="1411b-105">Офіс 365 бізнес і офіс 365 бізнес преміум плани не включають в себе офіс 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="1411b-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="1411b-106">Потрібно ввімкнути [активацію спільної комп'ютера](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="1411b-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="1411b-107">Якщо потрібно інсталювати Office 365 ProPlus на RDS з центру адміністрування Microsoft 365, ***який використовує параметри інсталяції за промовчанням***, виконайте такі дії:</span><span class="sxs-lookup"><span data-stu-id="1411b-107">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, follow these steps:</span></span>
  
1. <span data-ttu-id="1411b-108">Перевірте, який план Office 365 у вас є.</span><span class="sxs-lookup"><span data-stu-id="1411b-108">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="1411b-109">Дізнайтеся, як</span><span class="sxs-lookup"><span data-stu-id="1411b-109">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="1411b-110">У разі потреби переключіться на інший план Office 365.</span><span class="sxs-lookup"><span data-stu-id="1411b-110">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="1411b-111">Дізнайтеся, як</span><span class="sxs-lookup"><span data-stu-id="1411b-111">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="1411b-112">Якщо Office вже інстальовано на сервері RDS, використовуючи будь-які інші плани Office 365, видаліть його.</span><span class="sxs-lookup"><span data-stu-id="1411b-112">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="1411b-113">Наприклад, перейшовши на панель \> керування, видаліть програму.</span><span class="sxs-lookup"><span data-stu-id="1411b-113">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="1411b-114">Якщо ви працюєте з проблемами, видаліть за допомогою [служби підтримки Microsoft і помічника з відновлення](https://aka.ms/SARA-OfficeUninstall-Alchemy) .</span><span class="sxs-lookup"><span data-stu-id="1411b-114">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="1411b-115">На сервері RDS ввійдіть до центру адміністрування Microsoft 365 за допомогою облікового запису адміністратора та [інсталюйте Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="1411b-115">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="1411b-116">Після інсталяції Office ***не відкривайте або не входити в*** будь-які застосунки Office.</span><span class="sxs-lookup"><span data-stu-id="1411b-116">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="1411b-117">На сервері RDS Увімкніть спільна Активація комп'ютера за допомогою редагування реєстру, виконавши такі дії:</span><span class="sxs-lookup"><span data-stu-id="1411b-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="1411b-118">Клацніть правою кнопкою миші кнопку Windows у нижньому лівому куті екрана та виберіть пункт Виконати.</span><span class="sxs-lookup"><span data-stu-id="1411b-118">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="1411b-119">У полі "Відкрити" введіть **Regedit**і виберіть "OK".</span><span class="sxs-lookup"><span data-stu-id="1411b-119">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="1411b-120">Виберіть так, коли буде запропоновано дозволити редактору реєстру вносити зміни до пристрою.</span><span class="sxs-lookup"><span data-stu-id="1411b-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="1411b-121">У редакторі реєстру, додайте значення рядка **Sharedcomputer ліцензування** з настройки 1, під HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="1411b-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="1411b-122">На сервері RDS ***ввійдіть як кінцевий користувач*** і [Переконайтеся, що активація спільного комп'ютера увімкнуто для Office 365 proplus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="1411b-122">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="1411b-123">Щоб отримати додаткові відомості про попередні вимоги, інструкції з настроювання та вказівки щодо настроюваних інсталяцій за допомогою засобу розгортання Office, див. [розгортання Office 365 ProPlus за допомогою служб віддалених робочих столів](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="1411b-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="1411b-124">Щоб виправити помилки, пов'язані з активацією спільних комп'ютерів, перегляньте [Виправлення неполадок, пов'язаних із активацією спільних комп'ютерів для Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="1411b-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  