---
title: Виправлення неполадок під час реєстрації пристроїв Windows у Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 88105671ef6dc34553a265937bf1fb3463353963
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708911"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="f6a3e-102">Виправлення неполадок під час реєстрації пристроїв Windows у Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="f6a3e-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="f6a3e-103">Перегляньте наведені нижче ресурси, щоб вирішити проблему.</span><span class="sxs-lookup"><span data-stu-id="f6a3e-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="f6a3e-104">Деякі поширені повідомлення про помилки та роздільну здатність:</span><span class="sxs-lookup"><span data-stu-id="f6a3e-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="f6a3e-105">**Не вдалося інсталювати програмне забезпечення, 0x80cf4017:** Термін дії сертифіката облікового запису завершився.</span><span class="sxs-lookup"><span data-stu-id="f6a3e-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="f6a3e-106">Повторно завантажте пакет програмного забезпечення для клієнта ПК в консолі адміністратора Inune.</span><span class="sxs-lookup"><span data-stu-id="f6a3e-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="f6a3e-107">Перегляньте цю документацію, щоб отримати докладніші відомості.</span><span class="sxs-lookup"><span data-stu-id="f6a3e-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="f6a3e-108">**Код помилки 0x801c 0003:** Помилка може виникати в таких ситуаціях:</span><span class="sxs-lookup"><span data-stu-id="f6a3e-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="f6a3e-109">Користувач має більше пристроїв, зарахованих, ніж обмеження на пристрій.</span><span class="sxs-lookup"><span data-stu-id="f6a3e-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="f6a3e-110">Перегляньте ці документи, щоб [Видалити пристрій](https://docs.microsoft.com/intune/devices-wipe) або [Змінити обмеження на пристрій](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="f6a3e-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="f6a3e-111">"Користувачі можуть приєднатися до пристрою в Azure AD" "ні".</span><span class="sxs-lookup"><span data-stu-id="f6a3e-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="f6a3e-112">Установіть або виберіть елемент користувачі.</span><span class="sxs-lookup"><span data-stu-id="f6a3e-112">Set it to all or select users.</span></span> <span data-ttu-id="f6a3e-113">Перегляньте [цю документацію](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) , щоб отримати докладніші відомості.</span><span class="sxs-lookup"><span data-stu-id="f6a3e-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="f6a3e-114">Пристрій уже зареєстровано іншим користувачем.</span><span class="sxs-lookup"><span data-stu-id="f6a3e-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="f6a3e-115">Якщо це так, видаліть пристрій із консолі Azure Inune або вручну скасуйте реєстрацію пристрою, перш ніж намагатися ще раз.</span><span class="sxs-lookup"><span data-stu-id="f6a3e-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="f6a3e-116">Пристрій – це Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="f6a3e-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="f6a3e-117">Приєднатися до "Azure Active Directory" можна лише в ОС Windows 10 Pro, освіті та підприємстві SKUs.</span><span class="sxs-lookup"><span data-stu-id="f6a3e-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="f6a3e-118">Додаткові ресурси, які допоможуть вирішити проблему.</span><span class="sxs-lookup"><span data-stu-id="f6a3e-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="f6a3e-119">Використовуйте [портал виправлення неполадок](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , щоб діагностувати та усунути поширені помилки в реєстрації.</span><span class="sxs-lookup"><span data-stu-id="f6a3e-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="f6a3e-120">Перегляньте [цей документ](https://docs.microsoft.com/intune/help-desk-operators) , щоб отримати докладні відомості.</span><span class="sxs-lookup"><span data-stu-id="f6a3e-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="f6a3e-121">Перегляньте ці документи для списку поширених помилок, які перешкоджають виконанню та резолюціям кожного з них: [посібник із виправлення неполадок](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) і [Виправлення неполадок із документами](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="f6a3e-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="f6a3e-122">[Дізнайтеся, як зареєструвати пристрої Windows у Microsoft InTune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="f6a3e-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
