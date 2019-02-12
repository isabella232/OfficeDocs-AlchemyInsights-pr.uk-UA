---
title: Усунення несправностей із зарахування iOS пристроїв у Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: d28dca4fccf823e627dd179f828ba3b8baf843a6
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29924789"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="ccbc7-102">Усунення несправностей із зарахування iOS пристроїв у Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="ccbc7-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="ccbc7-103">Огляд ресурсів, перераховані нижче, щоб вирішити проблему, ваш тепер.</span><span class="sxs-lookup"><span data-stu-id="ccbc7-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="ccbc7-104">Деякі поширені повідомлення про помилки та резолюції кроки:</span><span class="sxs-lookup"><span data-stu-id="ccbc7-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="ccbc7-p101">**Пристрій обмеження досягнуто** Користувач має додаткові пристрої вступив ніж пристрою обмеження. Перегляньте ці документи до [зняття пристрою](https://docs.microsoft.com/intune/devices-wipe) або [Змінити обмеження на пристрій](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="ccbc7-p101">**Device Cap Reached** The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="ccbc7-p102">**Це послуга не підтримується. Немає реєстрації політика:** Apple підштовхнути служби сповіщень (APNS) повинен бути налаштований або знову. Огляд [цей документ](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) для отримання інструкцій про те, як це зробити.</span><span class="sxs-lookup"><span data-stu-id="ccbc7-p102">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed. Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="ccbc7-p103">**Користувача ліцензії типу неприпустиме або ім'я користувача не розпізнано:** Користувач повинен призначити Intune або EMS ліцензії. Перегляньте ці документи до призначите ліцензію через: [блакитні порталу](https://docs.microsoft.com/azure/active-directory/license-users-groups)або [Офісу Центру адміністрування](https://docs.microsoft.com/intune/licenses-assign) .</span><span class="sxs-lookup"><span data-stu-id="ccbc7-p103">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="ccbc7-111">Додаткові ресурси, щоб допомогти вирішити вашу проблему:</span><span class="sxs-lookup"><span data-stu-id="ccbc7-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="ccbc7-p104">Використовувати [Intune виправлення неполадок портал](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) діагностувати та усунути поширені зарахування невдач. Огляд [цей документ](https://docs.microsoft.com/intune/help-desk-operators) для більш докладної інформації.</span><span class="sxs-lookup"><span data-stu-id="ccbc7-p104">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="ccbc7-114">Перегляньте ці документи список поширених помилок, які заважають заявки на участь та постанов до кожного: [усунення несправностей керівництво](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) та [усунення несправностей doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="ccbc7-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="ccbc7-115">[Дізнайтеся, як записатися iOS пристроїв у Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="ccbc7-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

