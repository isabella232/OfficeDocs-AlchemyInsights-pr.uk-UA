---
title: Усунення проблем із зарахуванні iOS пристроїв у Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/18/2019
ms.locfileid: "36507024"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="329a4-102">Усунення проблем із зарахуванні iOS пристроїв у Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="329a4-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="329a4-103">Перегляньте ресурси, перелічені нижче, щоб вирішити проблему зараз.</span><span class="sxs-lookup"><span data-stu-id="329a4-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="329a4-104">Деякі поширені повідомлення про помилки та дії з роздільною здатністю:</span><span class="sxs-lookup"><span data-stu-id="329a4-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="329a4-105">**Досягнуто пристрою Cap** Користувач має більше пристроїв, що надійшли, ніж обмеження пристрою.</span><span class="sxs-lookup"><span data-stu-id="329a4-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="329a4-106">Перегляньте ці документи, щоб [Видалити пристрій](https://docs.microsoft.com/intune/devices-wipe) або [змінити ліміт пристрою](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="329a4-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="329a4-107">**Ця служба не підтримується. Немає реєстрації політика:** Apple Push повідомлення служби (APNS) необхідно налаштувати або поновити.</span><span class="sxs-lookup"><span data-stu-id="329a4-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="329a4-108">Перегляньте [цей документ](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) , щоб отримати інструкції щодо цього.</span><span class="sxs-lookup"><span data-stu-id="329a4-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="329a4-109">**Неприпустимий тип ліцензії для користувача або ім'я користувача, не розпізнано:** Користувачу потрібно призначити ліцензію InTune або EMS.</span><span class="sxs-lookup"><span data-stu-id="329a4-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="329a4-110">Перегляньте ці документи, щоб призначити ліцензію через: [Центр адміністрування Office](https://docs.microsoft.com/intune/licenses-assign) або [портал Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="329a4-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="329a4-111">Додаткові ресурси, які допоможуть вирішити проблему:</span><span class="sxs-lookup"><span data-stu-id="329a4-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="329a4-112">Для діагностики та вирішення поширених помилок реєстрації скористайтеся [InTune портал виправлення неполадок](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) .</span><span class="sxs-lookup"><span data-stu-id="329a4-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="329a4-113">Перегляньте [цей документ](https://docs.microsoft.com/intune/help-desk-operators) , щоб отримати докладніші відомості.</span><span class="sxs-lookup"><span data-stu-id="329a4-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="329a4-114">Перегляньте ці документи, щоб отримати список поширених помилок, які перешкоджають зарахуванням і роздільності до кожного: [посібник із виправлення неполадок](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) і [doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="329a4-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="329a4-115">[Дізнайтеся, як зареєструвати IOS пристроїв у Microsoft InTune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="329a4-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

