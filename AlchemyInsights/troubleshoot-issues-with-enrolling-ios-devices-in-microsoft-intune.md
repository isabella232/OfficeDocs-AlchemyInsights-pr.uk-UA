---
title: Виправлення неполадок під час реєстрації пристроїв з iOS у Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 7d3e0049258a77016250c8a657c8fbcaf8d65212
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47669269"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="9a539-102">Виправлення неполадок під час реєстрації пристроїв з iOS у Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="9a539-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="9a539-103">Перегляньте наведені нижче ресурси, щоб вирішити проблему.</span><span class="sxs-lookup"><span data-stu-id="9a539-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="9a539-104">Деякі поширені повідомлення про помилки та роздільну здатність:</span><span class="sxs-lookup"><span data-stu-id="9a539-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="9a539-105">Пристрій, на якому **досягнуто кришку** Користувач має більше пристроїв, зарахованих, ніж обмеження на пристрій.</span><span class="sxs-lookup"><span data-stu-id="9a539-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="9a539-106">Перегляньте ці документи, щоб [Видалити пристрій](https://docs.microsoft.com/intune/devices-wipe) або [Змінити обмеження на пристрій](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="9a539-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="9a539-107">**Ця служба не підтримується. Немає політики реєстрації:** ви повинні настроїти або поновити службу сповіщень Apple Push (APNS).</span><span class="sxs-lookup"><span data-stu-id="9a539-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="9a539-108">Перегляньте [цей документ](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) , щоб отримати вказівки щодо того, як це зробити.</span><span class="sxs-lookup"><span data-stu-id="9a539-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="9a539-109">**Неприпустимий тип ліцензії користувача або ім'я користувача не розпізнано:** Користувачу потрібно призначити ліцензію "Inune" або "EMS".</span><span class="sxs-lookup"><span data-stu-id="9a539-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="9a539-110">Перегляньте ці документи, щоб призначити ліцензію через: [Центр адміністрування Office](https://docs.microsoft.com/intune/licenses-assign) або [портал Azure Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="9a539-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="9a539-111">Додаткові ресурси, які допоможуть вирішити проблему.</span><span class="sxs-lookup"><span data-stu-id="9a539-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="9a539-112">Використовуйте [портал виправлення неполадок](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , щоб діагностувати та усунути поширені помилки в реєстрації.</span><span class="sxs-lookup"><span data-stu-id="9a539-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="9a539-113">Перегляньте [цей документ](https://docs.microsoft.com/intune/help-desk-operators) , щоб отримати докладні відомості.</span><span class="sxs-lookup"><span data-stu-id="9a539-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="9a539-114">Перегляньте ці документи для списку поширених помилок, які перешкоджають виконанню та резолюціям кожного з них: [посібник із виправлення неполадок](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) і [Виправлення неполадок із документами](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="9a539-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="9a539-115">[Дізнайтеся, як зареєструвати пристрої з iOS у Microsoft InTune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="9a539-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

