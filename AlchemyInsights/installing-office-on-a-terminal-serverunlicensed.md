---
title: Інсталяція Office на сервері терміналів-ліцензовано
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 7252efdc0f55b8923e685ec89f9b3c63882aa6b0
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763238"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="0db51-102">Інсталяція Office на сервері терміналів</span><span class="sxs-lookup"><span data-stu-id="0db51-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="0db51-103">Розгортання Microsoft 365 програм для підприємств на сервері Windows за допомогою служб віддалених робочих столів (RDS), раніше ім'я служби терміналів:</span><span class="sxs-lookup"><span data-stu-id="0db51-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="0db51-104">Потрібно мати передплату Microsoft 365, який містить програми Microsoft 365 для підприємств, наприклад Office 365 Enterprise E3 або Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="0db51-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="0db51-105">Програми Microsoft 365 для бізнесу та Microsoft 365 застосунки для бізнес-преміум плани не містять Microsoft 365 застосунки для підприємств.</span><span class="sxs-lookup"><span data-stu-id="0db51-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="0db51-106">Потрібно ввімкнути [активацію спільної комп'ютера](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="0db51-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="0db51-107">Якщо потрібно інсталювати програми Microsoft 365 для Enterprise на RDS з центру адміністрування Microsoft 365, ***який використовує параметри інсталяції за промовчанням***, виконайте такі дії.</span><span class="sxs-lookup"><span data-stu-id="0db51-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="0db51-108">Також можна завантажити та запустити помічника з [підтримки та відновлення Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) , щоб інсталювати програми Microsoft 365 для підприємств у режимі активації на спільному комп'ютері.</span><span class="sxs-lookup"><span data-stu-id="0db51-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="0db51-109">Перевірте, що ви маєте підписку Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0db51-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="0db51-110">Дізнайтеся, як</span><span class="sxs-lookup"><span data-stu-id="0db51-110">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="0db51-111">У разі потреби переключіться на іншу передплату Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0db51-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="0db51-112">Дізнайтеся, як</span><span class="sxs-lookup"><span data-stu-id="0db51-112">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="0db51-113">Якщо Office вже інстальовано на сервері RDS, використовуючи будь-які інші передплати Microsoft 365, видаліть його.</span><span class="sxs-lookup"><span data-stu-id="0db51-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="0db51-114">Наприклад, перейшовши на панель \> керування, видаліть програму.</span><span class="sxs-lookup"><span data-stu-id="0db51-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="0db51-115">Якщо ви працюєте з проблемами, видаліть за допомогою [служби підтримки Microsoft і помічника з відновлення](https://aka.ms/SARA-OfficeUninstall-Alchemy) .</span><span class="sxs-lookup"><span data-stu-id="0db51-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="0db51-116">На сервері RDS ввійдіть до центру адміністрування Microsoft 365 з обліковим записом адміністратора та [інсталюйте програми Microsoft 365 для підприємств](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="0db51-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="0db51-117">Після інсталяції Office ***не відкривайте або не входити в*** будь-які застосунки Office.</span><span class="sxs-lookup"><span data-stu-id="0db51-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="0db51-118">На сервері RDS Увімкніть спільна Активація комп'ютера за допомогою редагування реєстру, виконавши такі дії:</span><span class="sxs-lookup"><span data-stu-id="0db51-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="0db51-119">Клацніть правою кнопкою миші кнопку Windows у нижньому лівому куті екрана та виберіть пункт Виконати.</span><span class="sxs-lookup"><span data-stu-id="0db51-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="0db51-120">У полі "Відкрити" введіть **Regedit**і виберіть "OK".</span><span class="sxs-lookup"><span data-stu-id="0db51-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="0db51-121">Виберіть так, коли буде запропоновано дозволити редактору реєстру вносити зміни до пристрою.</span><span class="sxs-lookup"><span data-stu-id="0db51-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="0db51-122">У редакторі реєстру, додайте значення рядка **Sharedcomputer ліцензування** з настройки 1 у розділі HKEY_LOCAL_MACHINE \ програмне забезпеченя \ Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="0db51-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="0db51-123">На сервері RDS ***ввійдіть як кінцевий користувач*** і [Переконайтеся, що активація спільного комп'ютера увімкнуто для Microsoft 365 програм для підприємств](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="0db51-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="0db51-124">Щоб отримати додаткові відомості про попередні вимоги, інструкції з настроювання та вказівки щодо настроювання інсталяції за допомогою засобу розгортання Office, перегляньте [розгортання Microsoft 365 застосунки для підприємств за допомогою служб віддалених робочих столів](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="0db51-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="0db51-125">Щоб виправити помилки, пов'язані з активацією спільних комп'ютерів, перегляньте [вирішення проблем із активацією спільних комп'ютерів для програм Microsoft 365 для підприємств](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="0db51-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  