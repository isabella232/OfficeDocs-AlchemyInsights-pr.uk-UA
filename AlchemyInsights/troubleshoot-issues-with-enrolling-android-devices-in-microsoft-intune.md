---
title: Усунення несправностей із зарахування Android пристроїв у Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 2f4fc434128ebe7323f0b8c08aec3be82112bbda
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/24/2019
ms.locfileid: "29495754"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="783ec-102">Усунення несправностей із зарахування Android пристроїв у Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="783ec-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="783ec-103">Огляд ресурсів, перераховані нижче, щоб вирішити проблему, ваш тепер.</span><span class="sxs-lookup"><span data-stu-id="783ec-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="783ec-104">Деякі загальні питання і резолюції кроки:</span><span class="sxs-lookup"><span data-stu-id="783ec-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="783ec-p101">**Пристрої не зашифровані помилка на порталі компанії:** Новіші версії Android, особливо починаючи з v 7.0, вимагають запуску ввести пароль, щоб переконатися, що ваш пристрій повністю шифрується. Спільні рішення, щоб увімкнути автозавантаження PIN-код або повністю зашифрувати пристрою. Огляд [цей документ](https://docs.microsoft.com/en-us/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) для отримання додаткової інформації.</span><span class="sxs-lookup"><span data-stu-id="783ec-p101">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted. Common solutions are to enable a startup pin or fully encrypt the device. Review [this document](https://docs.microsoft.com/en-us/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span> 
  
 <span data-ttu-id="783ec-p102">**Пристрої не заглядати Intune служби або відобразити як "Нездорових" в консолі адміністратора Intune:** Деякі Samsung 4.4 і 5,5 пристроїв не можуть перевірити на службу. Існує 3 можливих рішень цієї проблеми:</span><span class="sxs-lookup"><span data-stu-id="783ec-p102">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service. There are 3 possible solutions to this issue:</span></span> 
  
1. <span data-ttu-id="783ec-110">Вручну відкрити портал компанії Intune програма, яка буде автоматично ініціювати пристрій синхронізації.</span><span class="sxs-lookup"><span data-stu-id="783ec-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>
    
2. <span data-ttu-id="783ec-111">Оновити пристрій Android 6.0 або вище.</span><span class="sxs-lookup"><span data-stu-id="783ec-111">Update the device to Android 6.0 or higher.</span></span>
    
3. <span data-ttu-id="783ec-p103">Вимкнути Samsung смарт-менеджер з управління портал компанії Intune. Огляд [цей документ](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) для більш докладної інформації з цих питань і резолюцій.</span><span class="sxs-lookup"><span data-stu-id="783ec-p103">Disable Samsung Smart Manager from managing the Intune Company Portal. Review [this document](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span> 
    
 <span data-ttu-id="783ec-p104">**Користувача ліцензії типу неприпустимий** або **користувач ім'я не розпізнано помилка:** що користувачеві необхідно призначити Intune або EMS ліцензії. Перегляньте ці документи до призначите ліцензію через: офіс центру адміністрування або Azure порталу.</span><span class="sxs-lookup"><span data-stu-id="783ec-p104">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span> 
  
<span data-ttu-id="783ec-116">Додаткові ресурси, щоб допомогти вирішити вашу проблему:</span><span class="sxs-lookup"><span data-stu-id="783ec-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="783ec-p105">Використовувати [Intune виправлення неполадок портал](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) діагностувати та усунути поширені зарахування невдач. Огляд [цей документ](https://docs.microsoft.com/en-us/intune/help-desk-operators) для більш докладної інформації.</span><span class="sxs-lookup"><span data-stu-id="783ec-p105">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/en-us/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="783ec-119">Огляд [цей документ](https://docs.microsoft.com/en-us/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) список поширених помилок, які заважають заявки на участь та постанов до кожного.</span><span class="sxs-lookup"><span data-stu-id="783ec-119">Review [this document](https://docs.microsoft.com/en-us/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span> 
    
3. <span data-ttu-id="783ec-120">[Дізнайтеся, як записатися Android пристроїв у Microsoft Intune](https://docs.microsoft.com/en-us/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="783ec-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/en-us/intune/android-enroll).</span></span>
    

