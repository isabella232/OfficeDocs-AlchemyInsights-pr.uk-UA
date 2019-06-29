---
title: Установка office сервера терміналів - неліцензійне
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
ms.openlocfilehash: 6fc4bd5f6971ca833084a6a8ad6c25b3fdafb8dc
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/28/2019
ms.locfileid: "35381750"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="933b2-102">Установка Office сервера терміналів</span><span class="sxs-lookup"><span data-stu-id="933b2-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="933b2-103">Для розгортання Office 365 ProPlus на сервері Windows за допомогою віддалений робочий стіл служб (РДС), раніше названий служб терміналів:</span><span class="sxs-lookup"><span data-stu-id="933b2-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="933b2-104">Ви повинні мати Office 365 план, який включає в себе Office 365 ProPlus, таких як Office 365 підприємство E3 або E5 підприємства.</span><span class="sxs-lookup"><span data-stu-id="933b2-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="933b2-105">Office 365 бізнесу та Office 365 бізнес преміум плани, не включають Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="933b2-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="933b2-106">Вам необхідно ввімкнути [спільний комп'ютер активації](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="933b2-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="933b2-107">Якщо потрібно інсталювати Office 365 ProPlus RDS на порталі Office 365, \* \* *який використовує за замовчуванням установки* \* \*, виконайте такі дії:</span><span class="sxs-lookup"><span data-stu-id="933b2-107">If you want to install Office 365 ProPlus on RDS from the Office 365 portal, \*\* *which uses default installation settings* \*\*, follow these steps:</span></span>
  
1. <span data-ttu-id="933b2-108">Перевірте, що плану Office 365.</span><span class="sxs-lookup"><span data-stu-id="933b2-108">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="933b2-109">Дізнайтеся, як</span><span class="sxs-lookup"><span data-stu-id="933b2-109">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="933b2-110">Якщо необхідно, переключитися на різних Office 365 плану.</span><span class="sxs-lookup"><span data-stu-id="933b2-110">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="933b2-111">Дізнайтеся, як</span><span class="sxs-lookup"><span data-stu-id="933b2-111">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="933b2-112">Якщо Office уже інстальовано на сервері RDS, використовуючи будь-які інші плани Office 365, видалити цей пакет оновлень.</span><span class="sxs-lookup"><span data-stu-id="933b2-112">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="933b2-113">Наприклад, перейшовши до панелі керування \> видалити програму.</span><span class="sxs-lookup"><span data-stu-id="933b2-113">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="933b2-114">Видаляється за допомогою [служби підтримки Microsoft і помічник відновлення](https://aka.ms/SARA-OfficeUninstall-Alchemy) , якщо ви працюєте в питаннях.</span><span class="sxs-lookup"><span data-stu-id="933b2-114">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="933b2-115">На сервері RDS ввійдіть до порталу Office 365 з вашим обліковим записом адміністратора і [установки Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="933b2-115">On the RDS server, sign in to the Office 365 portal with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="933b2-116">Після інсталяції Office, \* \* *не відкрити або увійдіть* \* \* до будь-якої програми Office.</span><span class="sxs-lookup"><span data-stu-id="933b2-116">After Office is installed, \*\* *don't open or sign in* \*\* to any Office applications.</span></span>

6. <span data-ttu-id="933b2-117">На сервері RDS увімкнути загальний комп'ютер активації за допомогою редагування реєстру, виконавши такі дії:</span><span class="sxs-lookup"><span data-stu-id="933b2-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="933b2-118">Клацніть правою кнопкою миші кнопку Windows в нижній лівий кут екрана та виберіть пункт запустити.</span><span class="sxs-lookup"><span data-stu-id="933b2-118">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="933b2-119">У полі Відкрити введіть **regedit**а потім виберіть ОК.</span><span class="sxs-lookup"><span data-stu-id="933b2-119">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="933b2-120">Виберіть так коли з'явиться запит на дозвіл редактор реєстру для внесення змін до пристрою.</span><span class="sxs-lookup"><span data-stu-id="933b2-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="933b2-121">У редакторі реєстру, додати Рядкове значення **SharedComputerLicensing** з настройкою 1 під HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="933b2-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="933b2-122">На сервері RDS \* \* *увійдіть як кінцевого користувача* \* \* і [Переконайтеся, що активація загальний комп'ютер увімкнуто для Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="933b2-122">On the RDS server, \*\* *sign in as an end user* \*\* and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="933b2-123">Для більш докладної інформації про передумови, інструкції з установки а також Указівки щодо налаштувати установки за допомогою засобу розгортання Office будь ласка, дивіться [Розгортати Office 365 ProPlus за допомогою служби віддалених робочих столів](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="933b2-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="933b2-124">Щоб виправити помилки, пов'язані з загальний комп'ютер активації, будь ласка, дивіться [питання виправлення неполадок з активацією загальний комп'ютер для Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="933b2-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  