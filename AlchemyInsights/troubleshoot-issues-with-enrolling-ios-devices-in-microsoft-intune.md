---
title: Усунення несправностей із записуванням пристроїв iOS у Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823484"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="2451a-102">Усунення несправностей із записуванням пристроїв iOS у Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="2451a-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="2451a-103">Перегляньте наведені нижче ресурси, щоб усунути проблему зараз.</span><span class="sxs-lookup"><span data-stu-id="2451a-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="2451a-104">Деякі типові повідомлення про помилки та кроки з їх усунення:</span><span class="sxs-lookup"><span data-stu-id="2451a-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="2451a-105">**Досягнуто максимальної потужності пристрою** Користувач має більше пристроїв, ніж максимальна кількість пристроїв.</span><span class="sxs-lookup"><span data-stu-id="2451a-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="2451a-106">Перегляньте ці [документи, щоб видалити пристрій](https://docs.microsoft.com/intune/devices-wipe) або змінити обмеження для [пристрою](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="2451a-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="2451a-107">**Ця служба не підтримується. Немає політики членство.** Потрібно налаштувати або поновити службу push-сповіщень Apple.</span><span class="sxs-lookup"><span data-stu-id="2451a-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="2451a-108">Перегляньте [цей документ,](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) щоб дізнатися, як це зробити.</span><span class="sxs-lookup"><span data-stu-id="2451a-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="2451a-109">**Неприпустимий тип ліцензії користувача або не розпізнано ім'я користувача:** Користувачу потрібно призначити ліцензію Intune або EMS.</span><span class="sxs-lookup"><span data-stu-id="2451a-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="2451a-110">Перегляньте ці документи, щоб призначити ліцензію через: [Центр адміністрування Office](https://docs.microsoft.com/intune/licenses-assign) або портал [Azure.](https://docs.microsoft.com/azure/active-directory/license-users-groups)</span><span class="sxs-lookup"><span data-stu-id="2451a-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="2451a-111">Додаткові ресурси, які допоможуть вирішити вашу проблему:</span><span class="sxs-lookup"><span data-stu-id="2451a-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="2451a-112">На [порталі виправлення неполадок Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) можна діагностувати та усунути поширені помилки входу.</span><span class="sxs-lookup"><span data-stu-id="2451a-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="2451a-113">Перегляньте [цей документ,](https://docs.microsoft.com/intune/help-desk-operators) щоб дізнатися більше.</span><span class="sxs-lookup"><span data-stu-id="2451a-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="2451a-114">Перегляньте ці документи, щоб отримати список типових помилок, які [](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) запобігають веденю та вирішене проблем із кожним [документом:](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)Посібник із виправлення неполадок і Виправлення неполадок.</span><span class="sxs-lookup"><span data-stu-id="2451a-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="2451a-115">[Дізнайтеся, як створити пристрої з iOS у Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)</span><span class="sxs-lookup"><span data-stu-id="2451a-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

