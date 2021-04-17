---
title: Усунення несправностей із записуванням пристроїв Android у Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830963"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="3a944-102">Усунення несправностей із записуванням пристроїв Android у Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="3a944-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="3a944-103">Перегляньте наведені нижче ресурси, щоб усунути проблему зараз.</span><span class="sxs-lookup"><span data-stu-id="3a944-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="3a944-104">Нижче наведено деякі поширені проблеми та спосіб вирішення.</span><span class="sxs-lookup"><span data-stu-id="3a944-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="3a944-105">**Помилка пристрою, не зашифрованого на порталі компанії:** Щоб повністю шифрувати пристрій, у новіших версіях Android, особливо починаючи з версії 7.0, потрібен код допуску.</span><span class="sxs-lookup"><span data-stu-id="3a944-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="3a944-106">Поширені рішення дають змогу ввімкнути pin-код запуску або повністю шифрувати пристрій.</span><span class="sxs-lookup"><span data-stu-id="3a944-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="3a944-107">Перегляньте [цей документ,](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) щоб отримати докладніші відомості.</span><span class="sxs-lookup"><span data-stu-id="3a944-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="3a944-108">Не вдається перевірити пристрій за допомогою служби Intune або відобразити стан "Несприятливий" у консолі **адміністратора Intune:** Деякі пристрої Samsung 4.4 та 5.5 можуть не потрапити до служби.</span><span class="sxs-lookup"><span data-stu-id="3a944-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="3a944-109">Цю проблему можна вирішити 3 способами:</span><span class="sxs-lookup"><span data-stu-id="3a944-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="3a944-110">Вручну відкрийте програму Intune Company Portal, яка автоматично ініціюватиме синхронізацію пристроїв.</span><span class="sxs-lookup"><span data-stu-id="3a944-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="3a944-111">Оновіть пристрій до Android 6.0 або новішої версії.</span><span class="sxs-lookup"><span data-stu-id="3a944-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="3a944-112">Вимкніть Samsung Smart Manager на порталі компанії Intune.</span><span class="sxs-lookup"><span data-stu-id="3a944-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="3a944-113">Перегляньте [цей документ,](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) щоб отримати додаткові відомості про ці проблеми та вирішення.</span><span class="sxs-lookup"><span data-stu-id="3a944-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="3a944-114">**Помилка "Тип ліцензії користувача"** Неприпустимий або Не розпізнано ім'я **користувача:** користувачу потрібно призначити ліцензію Intune або EMS.</span><span class="sxs-lookup"><span data-stu-id="3a944-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="3a944-115">Перегляньте ці документи, щоб призначити ліцензію через: Центр адміністрування Office або портал Azure.</span><span class="sxs-lookup"><span data-stu-id="3a944-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="3a944-116">Додаткові ресурси, які допоможуть вирішити вашу проблему:</span><span class="sxs-lookup"><span data-stu-id="3a944-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="3a944-117">На [порталі виправлення неполадок Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) можна діагностувати та усунути поширені помилки входу.</span><span class="sxs-lookup"><span data-stu-id="3a944-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="3a944-118">Перегляньте [цей документ,](https://docs.microsoft.com/intune/help-desk-operators) щоб дізнатися більше.</span><span class="sxs-lookup"><span data-stu-id="3a944-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="3a944-119">Перегляньте [цей документ,](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) щоб переглянути список типових помилок, які запобігають їй в списках і їх вирішення.</span><span class="sxs-lookup"><span data-stu-id="3a944-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="3a944-120">[Дізнайтеся, як затвердити пристрої Android у Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="3a944-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
