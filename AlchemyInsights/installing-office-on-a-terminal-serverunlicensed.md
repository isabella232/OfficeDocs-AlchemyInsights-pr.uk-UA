---
title: Інсталяція пакета Office на сервері терміналів – неліцензований
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663138"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="56659-102">Інсталяція пакета Office на сервері терміналів</span><span class="sxs-lookup"><span data-stu-id="56659-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="56659-103">Для розгортання програм Microsoft 365 для підприємств на сервері Windows Server за допомогою служб віддалених робочих столів (RDS), які раніше назвали служби терміналів:</span><span class="sxs-lookup"><span data-stu-id="56659-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="56659-104">Потрібно мати передплатну програму Microsoft 365, яка включає програми Microsoft 365 для підприємств, наприклад Office 365 Enterprise E3 або Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="56659-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="56659-105">У планах програми Microsoft 365 для бізнесу та програм Microsoft 365 для бізнесу Premium не включаються програми Microsoft 365 для підприємств.</span><span class="sxs-lookup"><span data-stu-id="56659-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="56659-106">Потрібно ввімкнути [активацію спільного комп'ютера](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="56659-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="56659-107">Якщо потрібно інсталювати програми Microsoft 365 для підприємств на RDS у центрі адміністрування Microsoft 365, у ***якому використовуються стандартні параметри інсталяції***, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="56659-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="56659-108">Ви також можете завантажити та запустити [помічник із підтримки й відновлення Microsoft,](https://aka.ms/SaRA_OfficeSCA_M365Portal) щоб інсталювати програми Microsoft 365 для підприємств у режимі активації спільного комп'ютера.</span><span class="sxs-lookup"><span data-stu-id="56659-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="56659-109">Перевірте, що таке Передплата на Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="56659-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="56659-110">Дізнайтеся, як</span><span class="sxs-lookup"><span data-stu-id="56659-110">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="56659-111">Якщо потрібно, перейдіть до іншої абонентської плати Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="56659-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="56659-112">Дізнайтеся, як</span><span class="sxs-lookup"><span data-stu-id="56659-112">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. <span data-ttu-id="56659-113">Якщо пакет Office уже інстальовано на сервері RDS, використовуючи будь-які інші передплати Microsoft 365, видаліть його.</span><span class="sxs-lookup"><span data-stu-id="56659-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="56659-114">Наприклад, вибравши панель керування, \> видаліть програму.</span><span class="sxs-lookup"><span data-stu-id="56659-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="56659-115">Ви можете видалити за допомогою [помічника з підтримки й відновлення Microsoft,](https://aka.ms/SARA-OfficeUninstall-Alchemy) якщо ви працюєте з проблемами.</span><span class="sxs-lookup"><span data-stu-id="56659-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="56659-116">На сервері RDS Увійдіть у центр адміністрування Microsoft 365 за допомогою облікового запису адміністратора та [інсталюйте програми Microsoft 365 для підприємств](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="56659-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="56659-117">Після інсталяції Office ***не відкривайте та не ввійдіть в*** будь-які програми Office.</span><span class="sxs-lookup"><span data-stu-id="56659-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="56659-118">На сервері RDS Увімкніть активацію спільного комп'ютера, змінивши реєстр, виконавши наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="56659-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="56659-119">Клацніть правою кнопкою миші кнопку Windows у лівому нижньому куті екрана, а потім виберіть команду виконати.</span><span class="sxs-lookup"><span data-stu-id="56659-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="56659-120">У полі Відкрити введіть **Regedit**, а потім натисніть кнопку OK.</span><span class="sxs-lookup"><span data-stu-id="56659-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="56659-121">Натисніть кнопку Так, коли з'явиться запит на дозвіл редактор реєстру, щоб внести зміни до вашого пристрою.</span><span class="sxs-lookup"><span data-stu-id="56659-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="56659-122">У редакторі реєстру додайте рядне значення для **Sharedcompuitліцензування** з параметром 1 в розділі HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="56659-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="56659-123">На сервері RDS ***увійдіть як кінцевий користувач*** і [Переконайтеся, що активовано функцію активації спільного комп'ютера для програм Microsoft 365 для підприємств](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="56659-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="56659-124">Докладні відомості про попередні вимоги, інструкції з настроювання та вказівки щодо настроюваних інсталяцій за допомогою засобу розгортання Office наведено в статті [розгортання програм Microsoft 365 для підприємств за допомогою служб віддаленого робочого стола](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="56659-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="56659-125">Щоб виправити помилки, пов'язані з активацією на спільному комп'ютері, ознайомтеся [з проблемами усунення проблем із підключенням до спільного комп'ютера для програм Microsoft 365 для підприємств](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="56659-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  