---
title: Установка office сервера терміналів - неліцензійне
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 971edd9c064b448446ba16361e99df4a2291c14f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29919005"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="55f58-102">Установка Office сервера терміналів</span><span class="sxs-lookup"><span data-stu-id="55f58-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="55f58-103">Для розгортання Office 365 ProPlus на сервері Windows за допомогою віддалений робочий стіл служб (РДС), раніше названий служб терміналів:</span><span class="sxs-lookup"><span data-stu-id="55f58-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="55f58-p101">Ви повинні мати Office 365 план, який включає в себе Office 365 ProPlus, таких як Office 365 підприємство E3 або E5 підприємства. Office 365 бізнесу та Office 365 бізнес преміум плани, не включають Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="55f58-p101">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5. The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
    
- <span data-ttu-id="55f58-106">Вам необхідно ввімкнути [спільний комп'ютер активації](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="55f58-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>
    
<span data-ttu-id="55f58-107">Якщо потрібно інсталювати Office 365 ProPlus RDS на порталі Office 365, \* \* *який використовує за замовчуванням установки* \* \*, виконайте такі дії:</span><span class="sxs-lookup"><span data-stu-id="55f58-107">If you want to install Office 365 ProPlus on RDS from the Office 365 portal, \*\* *which uses default installation settings* \*\*, follow these steps:</span></span> 
  
1. <span data-ttu-id="55f58-p102">Перевірте, що плану Office 365. [ЖЖ як](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)</span><span class="sxs-lookup"><span data-stu-id="55f58-p102">Check what Office 365 plan you have. [Learn how](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)</span></span>
    
2. <span data-ttu-id="55f58-p103">Якщо необхідно, переключитися на різних Office 365 плану. [ЖЖ як](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)</span><span class="sxs-lookup"><span data-stu-id="55f58-p103">If necessary, switch to a different Office 365 plan. [Learn how](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)</span></span>
    
3. <span data-ttu-id="55f58-p104">Якщо Office уже інстальовано на сервері RDS, використовуючи будь-які інші плани Office 365, видалити цей пакет оновлень. Наприклад, перейшовши до панелі керування \> видалити програму. Видаляється за допомогою [служби підтримки Microsoft і помічник відновлення](https://aka.ms/SARA-OfficeUninstall-Alchemy) , якщо ви працюєте в питаннях.</span><span class="sxs-lookup"><span data-stu-id="55f58-p104">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it. For example, by going to Control Panel \> Uninstall a program. Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span> 
    
4. <span data-ttu-id="55f58-115">На сервері RDS ввійдіть до порталу Office 365 з вашим обліковим записом адміністратора і [установки Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="55f58-115">On the RDS server, sign in to the Office 365 portal with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
    
5. <span data-ttu-id="55f58-116">Після інсталяції Office, \* \* *не відкрити або увійдіть* \* \* до будь-якої програми Office.</span><span class="sxs-lookup"><span data-stu-id="55f58-116">After Office is installed, \*\* *don't open or sign in* \*\* to any Office applications.</span></span> 
    
6. <span data-ttu-id="55f58-117">На сервері RDS увімкнути загальний комп'ютер активації за допомогою редагування реєстру, виконавши такі дії:</span><span class="sxs-lookup"><span data-stu-id="55f58-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
    
1. <span data-ttu-id="55f58-p105">Клацніть правою кнопкою миші кнопку Windows в нижній лівий кут екрана та виберіть пункт запустити. У полі Відкрити введіть **regedit**а потім виберіть ОК.</span><span class="sxs-lookup"><span data-stu-id="55f58-p105">Right-click the Windows button in the lower left-hand corner of your screen and select Run. In the Open box, type **regedit**, and then select OK.</span></span> 
    
2. <span data-ttu-id="55f58-120">Виберіть так коли з'явиться запит на дозвіл редактор реєстру для внесення змін до пристрою.</span><span class="sxs-lookup"><span data-stu-id="55f58-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>
    
3. <span data-ttu-id="55f58-121">У редакторі реєстру, додати Рядкове значення **SharedComputerLicensing** з настройкою 1 під HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="55f58-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span> 
    
7. <span data-ttu-id="55f58-122">На сервері RDS \* \* *увійдіть як кінцевого користувача* \* \* і [Переконайтеся, що активація загальний комп'ютер увімкнуто для Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="55f58-122">On the RDS server, \*\* *sign in as an end user* \*\* and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>
    
<span data-ttu-id="55f58-123">Для більш докладної інформації про передумови, інструкції з установки а також Указівки щодо налаштувати установки за допомогою засобу розгортання Office будь ласка, дивіться [Розгортати Office 365 ProPlus за допомогою служби віддалених робочих столів](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="55f58-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="55f58-124">Щоб виправити помилки, пов'язані з загальний комп'ютер активації, будь ласка, дивіться [питання виправлення неполадок з активацією загальний комп'ютер для Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="55f58-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  

