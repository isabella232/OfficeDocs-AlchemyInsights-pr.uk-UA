---
title: Усунення несправностей із записуванням пристроїв Windows у Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a456cc8f2336e6b902de0b7873cb233f4b846140
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51808992"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="6a23d-102">Усунення несправностей із записуванням пристроїв Windows у Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="6a23d-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="6a23d-103">Перегляньте наведені нижче ресурси, щоб усунути проблему зараз.</span><span class="sxs-lookup"><span data-stu-id="6a23d-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="6a23d-104">Деякі типові повідомлення про помилки та кроки з їх усунення:</span><span class="sxs-lookup"><span data-stu-id="6a23d-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="6a23d-105">**Програмне забезпечення не можна інсталювати, 0x80cf4017:** Термін дії сертифіката вашого облікового запису минув.</span><span class="sxs-lookup"><span data-stu-id="6a23d-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="6a23d-106">Повторно завантажте пакет програмного забезпечення "Клієнт ПК" у консолі адміністратора Intune.</span><span class="sxs-lookup"><span data-stu-id="6a23d-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="6a23d-107">Докладні відомості див. в цій документації.</span><span class="sxs-lookup"><span data-stu-id="6a23d-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="6a23d-108">**Код помилки 0x801c0003:** Помилка може статися в таких випадках:</span><span class="sxs-lookup"><span data-stu-id="6a23d-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="6a23d-109">Користувач має більше пристроїв, ніж максимальна кількість пристроїв.</span><span class="sxs-lookup"><span data-stu-id="6a23d-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="6a23d-110">Перегляньте ці [документи, щоб видалити пристрій](https://docs.microsoft.com/intune/devices-wipe) або змінити обмеження для [пристрою](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="6a23d-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="6a23d-111">Для параметра "Користувачі можуть приєднуватися до пристроїв до Azure AD" установлено значення "немає".</span><span class="sxs-lookup"><span data-stu-id="6a23d-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="6a23d-112">Настройте її для всіх або кількох користувачів.</span><span class="sxs-lookup"><span data-stu-id="6a23d-112">Set it to all or select users.</span></span> <span data-ttu-id="6a23d-113">Докладні [відомості див. в](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) цій документації.</span><span class="sxs-lookup"><span data-stu-id="6a23d-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="6a23d-114">Інший користувач уже затвердив пристрій.</span><span class="sxs-lookup"><span data-stu-id="6a23d-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="6a23d-115">У такому разі видаліть пристрій із консолі Azure Intune або вручну спустіть пристрій, перш ніж повторити спробу.</span><span class="sxs-lookup"><span data-stu-id="6a23d-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="6a23d-116">Пристрій – це Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="6a23d-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="6a23d-117">До Azure Active Directory можуть приєднатися лише облікові номери Windows 10 Pro, Education і Enterprise.</span><span class="sxs-lookup"><span data-stu-id="6a23d-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="6a23d-118">Додаткові ресурси, які допоможуть вирішити вашу проблему:</span><span class="sxs-lookup"><span data-stu-id="6a23d-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="6a23d-119">На [порталі виправлення неполадок Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) можна діагностувати та усунути поширені помилки входу.</span><span class="sxs-lookup"><span data-stu-id="6a23d-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="6a23d-120">Перегляньте [цей документ,](https://docs.microsoft.com/intune/help-desk-operators) щоб дізнатися більше.</span><span class="sxs-lookup"><span data-stu-id="6a23d-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="6a23d-121">Перегляньте ці документи, щоб отримати список типових помилок, які [](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) запобігають веденю та вирішене проблем із кожним [документом:](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)Посібник із виправлення неполадок і Виправлення неполадок.</span><span class="sxs-lookup"><span data-stu-id="6a23d-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="6a23d-122">[Дізнайтеся, як створити обліковий запис для пристроїв Windows у Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)</span><span class="sxs-lookup"><span data-stu-id="6a23d-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
