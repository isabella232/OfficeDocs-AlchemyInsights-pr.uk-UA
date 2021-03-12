---
title: Виправлення неполадок під час реєстрації пристроїв на платформі Android у Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: cc8c68a1e838f67c4510002b2c7ff5294a4649fe
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709019"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="f11b6-102">Виправлення неполадок під час реєстрації пристроїв на платформі Android у Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="f11b6-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="f11b6-103">Перегляньте наведені нижче ресурси, щоб вирішити проблему.</span><span class="sxs-lookup"><span data-stu-id="f11b6-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="f11b6-104">Деякі поширені проблеми та вказівки з вирішення:</span><span class="sxs-lookup"><span data-stu-id="f11b6-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="f11b6-105">**Пристрій не зашифрована помилка на порталі компанії:** Новіші версії Android, зокрема, починаючи з v 7.0, вимагають код запуску, щоб переконатися, що пристрій повністю зашифровано.</span><span class="sxs-lookup"><span data-stu-id="f11b6-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="f11b6-106">Загальні рішення дають змогу активувати PIN-код або повністю зашифрувати пристрій.</span><span class="sxs-lookup"><span data-stu-id="f11b6-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="f11b6-107">Перегляньте [цей документ](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) , щоб отримати докладні відомості.</span><span class="sxs-lookup"><span data-stu-id="f11b6-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="f11b6-108">**Не вдається виконати вхід за допомогою служби InTune або відображення як "нездорові" в консолі адміністрування inune:** Деякі пристрої Samsung 4,4 і 5,5 можуть не перевіряти в службу.</span><span class="sxs-lookup"><span data-stu-id="f11b6-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="f11b6-109">Цю проблему наведено в трьох можливих варіантів:</span><span class="sxs-lookup"><span data-stu-id="f11b6-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="f11b6-110">Вручну відкрийте програму "портал компанії", яка автоматично ініціюватиме синхронізацію пристрою.</span><span class="sxs-lookup"><span data-stu-id="f11b6-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="f11b6-111">Оновіть пристрій до Android 6,0 або новішої версії.</span><span class="sxs-lookup"><span data-stu-id="f11b6-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="f11b6-112">Вимкніть програму Samsung Smart Manager від керування порталом компанії Inune.</span><span class="sxs-lookup"><span data-stu-id="f11b6-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="f11b6-113">Перегляньте [цей документ](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) , щоб отримати докладні відомості про ці проблеми та способи вирішення.</span><span class="sxs-lookup"><span data-stu-id="f11b6-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="f11b6-114">Помилка **типу ліцензії користувача** або **ім'я користувача не розпізнано:** користувач має бути призначений ЛІЦЕНЗІЄЮ inune або EMS.</span><span class="sxs-lookup"><span data-stu-id="f11b6-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="f11b6-115">Перегляньте ці документи, щоб призначити ліцензію через: Центр адміністрування Office або портал Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="f11b6-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="f11b6-116">Додаткові ресурси, які допоможуть вирішити проблему.</span><span class="sxs-lookup"><span data-stu-id="f11b6-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="f11b6-117">Використовуйте [портал виправлення неполадок](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , щоб діагностувати та усунути поширені помилки в реєстрації.</span><span class="sxs-lookup"><span data-stu-id="f11b6-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="f11b6-118">Перегляньте [цей документ](https://docs.microsoft.com/intune/help-desk-operators) , щоб отримати докладні відомості.</span><span class="sxs-lookup"><span data-stu-id="f11b6-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="f11b6-119">Перегляньте [цей документ](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) для списку поширених помилок, які перешкоджають виконанню та дозволах для кожного з них.</span><span class="sxs-lookup"><span data-stu-id="f11b6-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="f11b6-120">[Дізнайтеся, як зареєструвати пристрої Android у Microsoft InTune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="f11b6-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
