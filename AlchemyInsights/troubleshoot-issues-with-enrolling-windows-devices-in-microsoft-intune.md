---
title: Усунення проблем із зарахуванні пристроїв Windows у Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665853"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="aad64-102">Усунення проблем із зарахуванні пристроїв Windows у Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="aad64-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="aad64-103">Перегляньте ресурси, перелічені нижче, щоб вирішити проблему зараз.</span><span class="sxs-lookup"><span data-stu-id="aad64-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="aad64-104">Деякі поширені повідомлення про помилки та дії з роздільною здатністю:</span><span class="sxs-lookup"><span data-stu-id="aad64-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="aad64-105">**Не вдається встановити програмне забезпечення, 0x80cf4017:** Термін дії сертифіката облікового запису минув.</span><span class="sxs-lookup"><span data-stu-id="aad64-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="aad64-106">Повторно завантажити пакет клієнтського програмного забезпечення для комп'ютера, InTune консолі адміністратора.</span><span class="sxs-lookup"><span data-stu-id="aad64-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="aad64-107">Перегляньте цю документацію, щоб отримати докладнішу інформацію.</span><span class="sxs-lookup"><span data-stu-id="aad64-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="aad64-108">**Код помилки 0x801c0003:** Повідомлення про помилку може виникнути в таких випадках:</span><span class="sxs-lookup"><span data-stu-id="aad64-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="aad64-109">Користувач має більше пристроїв, що надійшли, ніж обмеження пристрою.</span><span class="sxs-lookup"><span data-stu-id="aad64-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="aad64-110">Перегляньте ці документи, щоб [Видалити пристрій](https://docs.microsoft.com/intune/devices-wipe) або [змінити ліміт пристрою](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="aad64-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="aad64-111">"Користувачі можуть приєднатися до пристроїв Azure AD" встановлено "немає".</span><span class="sxs-lookup"><span data-stu-id="aad64-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="aad64-112">Встановіть його на всі або виберіть користувачів.</span><span class="sxs-lookup"><span data-stu-id="aad64-112">Set it to all or select users.</span></span> <span data-ttu-id="aad64-113">Перегляньте [цю документацію](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) , щоб отримати докладнішу інформацію.</span><span class="sxs-lookup"><span data-stu-id="aad64-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="aad64-114">Пристрій уже зареєстровано іншим користувачем.</span><span class="sxs-lookup"><span data-stu-id="aad64-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="aad64-115">Якщо це так, вийміть пристрій із консолі Azure InTune або вручну скасувати реєстрації пристрою перед повторною спробою.</span><span class="sxs-lookup"><span data-stu-id="aad64-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="aad64-116">Пристрій Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="aad64-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="aad64-117">Тільки Windows 10 Pro, освіта і підприємство SKUs може приєднатися до Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="aad64-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="aad64-118">Додаткові ресурси, які допоможуть вирішити проблему:</span><span class="sxs-lookup"><span data-stu-id="aad64-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="aad64-119">Для діагностики та вирішення поширених помилок реєстрації скористайтеся [InTune портал виправлення неполадок](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) .</span><span class="sxs-lookup"><span data-stu-id="aad64-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="aad64-120">Перегляньте [цей документ](https://docs.microsoft.com/intune/help-desk-operators) , щоб отримати докладніші відомості.</span><span class="sxs-lookup"><span data-stu-id="aad64-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="aad64-121">Перегляньте ці документи, щоб отримати список поширених помилок, які перешкоджають зарахуванням і роздільності до кожного: [посібник із виправлення неполадок](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) і [doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="aad64-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="aad64-122">[Дізнайтеся, як зареєструвати пристрої Windows у програмі Microsoft InTune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="aad64-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
