---
title: Усунення несправностей із зарахування пристроїв Windows у корпорації Майкрософт Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8d19bbd5a5782c7793c87499baf62b2eb7de82ae
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/24/2019
ms.locfileid: "29495891"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="582ef-102">Усунення несправностей із зарахування пристроїв Windows у корпорації Майкрософт Intune</span><span class="sxs-lookup"><span data-stu-id="582ef-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="582ef-103">Огляд ресурсів, перераховані нижче, щоб вирішити проблему, ваш тепер.</span><span class="sxs-lookup"><span data-stu-id="582ef-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="582ef-104">Деякі поширені повідомлення про помилки та резолюції кроки:</span><span class="sxs-lookup"><span data-stu-id="582ef-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="582ef-p101">**Не вдалося інсталювати програмне забезпечення, 0x80cf4017:** Ваш обліковий запис сертифіката закінчився. Повторно завантажити пакет програмного забезпечення ПК клієнта в консолі адміністратора Intune. Огляд цієї документації для отримання додаткової інформації.</span><span class="sxs-lookup"><span data-stu-id="582ef-p101">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired. Re-download the PC Client software package in the Intune Admin Console. Review this documentation for more information.</span></span> 
  
 <span data-ttu-id="582ef-108">**Код помилки 0x801c0003:** Помилка може виникнути у таких випадках:</span><span class="sxs-lookup"><span data-stu-id="582ef-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span> 
  
1. <span data-ttu-id="582ef-p102">Користувач має додаткові пристрої вступив ніж пристрою обмеження. Перегляньте ці документи до [зняття пристрою](https://docs.microsoft.com/en-us/intune/devices-wipe) або [Змінити обмеження на пристрій](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="582ef-p102">The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/en-us/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
2. <span data-ttu-id="582ef-p103">"Користувачі можуть приєднатися до пристроїв блакитні об'яви" встановлено значення "немає". Встановіть його на всіх, або виберіть користувачів. Огляд [цієї документації](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) для отримання додаткової інформації.</span><span class="sxs-lookup"><span data-stu-id="582ef-p103">"Users may join devices to Azure AD" is set to "none". Set it to all or select users. Review [this documentation](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span> 
    
3. <span data-ttu-id="582ef-p104">Пристрою вже зареєстровано іншим користувачем. Якщо це так, видалити пристрій з Azure Intune консоль або вручну unenroll пристрій, перш ніж повторити спробу.</span><span class="sxs-lookup"><span data-stu-id="582ef-p104">The device is already enrolled by another user. If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>
    
4. <span data-ttu-id="582ef-p105">Становить 10 Windows Home. Тільки Windows 10 Pro, освіти та рішенню щодо підприємства можуть приєднатися до Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="582ef-p105">The device is Windows 10 Home. Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>
    
<span data-ttu-id="582ef-118">Додаткові ресурси, щоб допомогти вирішити вашу проблему:</span><span class="sxs-lookup"><span data-stu-id="582ef-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="582ef-p106">Використовувати [Intune виправлення неполадок портал](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) діагностувати та усунути поширені зарахування невдач. Огляд [цей документ](https://docs.microsoft.com/en-us/intune/help-desk-operators) для більш докладної інформації.</span><span class="sxs-lookup"><span data-stu-id="582ef-p106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/en-us/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="582ef-121">Перегляньте ці документи список поширених помилок, які заважають заявки на участь та постанов до кожного: [усунення несправностей керівництво](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) та [усунення несправностей doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="582ef-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
<span data-ttu-id="582ef-122">[Дізнайтеся, як записатися пристроїв Windows у корпорації Майкрософт Intune](https://docs.microsoft.com/en-us/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="582ef-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/en-us/intune/windows-enroll).</span></span>
  

