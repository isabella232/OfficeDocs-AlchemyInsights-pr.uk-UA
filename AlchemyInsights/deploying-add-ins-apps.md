---
title: Розгортання надбудов для Програми Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233555"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="59c05-102">Розгортання надбудов для Програми Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="59c05-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="59c05-103">Централізоване розгортання – рекомендований спосіб розгортання Office надбудов для користувачів і груп в організації.</span><span class="sxs-lookup"><span data-stu-id="59c05-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="59c05-104">Щоб розгорнути надбудови, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="59c05-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="59c05-105">**Примітка.** Відомості про інсталяцію надбудов Office як окремого користувача див. в статті Перегляд і інсталяція надбудов, а також керування [ними Office програмах.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)</span><span class="sxs-lookup"><span data-stu-id="59c05-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="59c05-106">Крім того, переконайтеся, що окреме придбання Office Надбудови з Магазину увімкнуто.</span><span class="sxs-lookup"><span data-stu-id="59c05-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> <span data-ttu-id="59c05-107">Докладні відомості див. в розділі Запобігання завантаженню надбудов, вимкнувши Магазин Office в усіх клієнтах [(крім Outlook).](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)</span><span class="sxs-lookup"><span data-stu-id="59c05-107">For details, see [Prevent add-in downloads by turning off the Office Store across all clients (Except Outlook)](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook).</span></span>

1. <span data-ttu-id="59c05-108">Переконайтеся, що середовище відповідає вимогам до розгортання надбудов за допомогою централізованого розгортання.</span><span class="sxs-lookup"><span data-stu-id="59c05-108">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="59c05-109">Докладніші відомості див. у [шкалику Вимоги](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span><span class="sxs-lookup"><span data-stu-id="59c05-109">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="59c05-110">Перейдіть до **Настройки**  >  **Інтегровані** програми Завантажити  >  **програми** Microsoft 365, щоб розгорнути надбудови.</span><span class="sxs-lookup"><span data-stu-id="59c05-110">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="59c05-111">Примітки.</span><span class="sxs-lookup"><span data-stu-id="59c05-111">Notes:</span></span> 

- <span data-ttu-id="59c05-112">Щоб інтегрувати програми, адміністратор має дозволи глобального адміністратора Exchange адміністраторів.</span><span class="sxs-lookup"><span data-stu-id="59c05-112">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="59c05-113">Розгортаючи надбудови для кількох користувачів, радимо робити завдання за допомогою груп, а не окремих користувачів.</span><span class="sxs-lookup"><span data-stu-id="59c05-113">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="59c05-114">Докладні відомості див. в статтях Рекомендації щодо призначення [надбудови користувачам і групам.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)</span><span class="sxs-lookup"><span data-stu-id="59c05-114">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="59c05-115">Централізоване розгортання не підтримує користувачів у вкладених групах або групах, які мають батьківські групи.</span><span class="sxs-lookup"><span data-stu-id="59c05-115">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="59c05-116">Докладні відомості [див. в цьому посібнику: призначення користувачів і груп.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)</span><span class="sxs-lookup"><span data-stu-id="59c05-116">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="59c05-117">Переконайтеся, що службу керування програмами Microsoft 365 (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') увімкнуто для користувачів для входу.</span><span class="sxs-lookup"><span data-stu-id="59c05-117">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="59c05-118">Докладні відомості див. [в цьому вікні.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)</span><span class="sxs-lookup"><span data-stu-id="59c05-118">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="59c05-119">Якщо під час розгортання надбудов виникають проблеми з розгортанням за допомогою функції "Інтегровані програми", спробуйте розгорнути [їх за допомогою надбудов.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)</span><span class="sxs-lookup"><span data-stu-id="59c05-119">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="59c05-120">Докладні відомості:</span><span class="sxs-lookup"><span data-stu-id="59c05-120">For more information, see:</span></span>

<span data-ttu-id="59c05-121">[Розгортання надбудов у Центрі адміністрування](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Керування надбудовами в Центрі адміністрування](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 Керування надбудовами за допомогою командлетів [PowerShell централізованого розгортання](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Публікування Office надбудов за допомогою централізованого](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) розгортання в Центрі Microsoft 365 адміністрування 
 [Усунення несправностей: Користувач не бачить надбудови](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Виправлення помилок користувачів Office надбудовах](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="59c05-121">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>