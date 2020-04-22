---
title: Усунення проблем із зарахуванні пристроїв Android у Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759641"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="d6250-102">Усунення проблем із зарахуванні пристроїв Android у Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="d6250-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="d6250-103">Перегляньте ресурси, перелічені нижче, щоб вирішити проблему зараз.</span><span class="sxs-lookup"><span data-stu-id="d6250-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="d6250-104">Деякі поширені проблеми та вирішення кроки:</span><span class="sxs-lookup"><span data-stu-id="d6250-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="d6250-105">**Пристрій не зашифрована помилка в порталі компанії:** Новіші версії Android, зокрема починаючи з версії 7.0, вимагають завантаження пароля, щоб переконатися, що пристрій повністю зашифровано.</span><span class="sxs-lookup"><span data-stu-id="d6250-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="d6250-106">Загальними рішеннями є ввімкнення PIN-коду або повного шифрування пристрою.</span><span class="sxs-lookup"><span data-stu-id="d6250-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="d6250-107">Перегляньте [цей документ](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) , щоб отримати додаткові відомості.</span><span class="sxs-lookup"><span data-stu-id="d6250-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="d6250-108">**Пристрої не вдається перевірити за допомогою служби InTune або відображення як "нездоровий" у консолі адміністратора InTune:** Деякі пристрої Samsung 4,4 та 5,5 можуть не перевіряти в сервісі.</span><span class="sxs-lookup"><span data-stu-id="d6250-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="d6250-109">Є 3 варіанти вирішення цієї проблеми:</span><span class="sxs-lookup"><span data-stu-id="d6250-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="d6250-110">Вручну відкрийте програму портал компанії InTune, яка автоматично ініціюватиме синхронізацію пристрою.</span><span class="sxs-lookup"><span data-stu-id="d6250-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="d6250-111">Оновіть пристрій до Android 6,0 або новішої.</span><span class="sxs-lookup"><span data-stu-id="d6250-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="d6250-112">Вимкніть Samsung Smart Manager, з керування портал компанії InTune.</span><span class="sxs-lookup"><span data-stu-id="d6250-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="d6250-113">Перегляньте [цей документ](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) , щоб отримати додаткові відомості про ці проблеми та рішення.</span><span class="sxs-lookup"><span data-stu-id="d6250-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="d6250-114">**Неприпустимий тип ліцензії** або **ім'я користувача не розпізнано помилка:** користувачу необхідно ПРИЗНАЧИТИ ліцензію InTune або EMS.</span><span class="sxs-lookup"><span data-stu-id="d6250-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="d6250-115">Перегляньте ці документи, щоб призначити ліцензію через: Центр адміністрування Office або портал Azure.</span><span class="sxs-lookup"><span data-stu-id="d6250-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="d6250-116">Додаткові ресурси, які допоможуть вирішити проблему:</span><span class="sxs-lookup"><span data-stu-id="d6250-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="d6250-117">Для діагностики та вирішення поширених помилок реєстрації скористайтеся [InTune портал виправлення неполадок](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) .</span><span class="sxs-lookup"><span data-stu-id="d6250-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="d6250-118">Перегляньте [цей документ](https://docs.microsoft.com/intune/help-desk-operators) , щоб отримати докладніші відомості.</span><span class="sxs-lookup"><span data-stu-id="d6250-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="d6250-119">Перегляньте [цей документ](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) для списку поширених помилок, які перешкоджають реєстрації та роздільності.</span><span class="sxs-lookup"><span data-stu-id="d6250-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="d6250-120">[Дізнайтеся, як зареєструвати Android пристроїв у Microsoft InTune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="d6250-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
