---
title: Усунення несправностей із зарахування Android пристроїв у Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 1e1d50c31df588a3416d758d40fbd7bde3f73b21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36500092"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="d6929-102">Усунення несправностей із зарахування Android пристроїв у Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="d6929-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="d6929-103">Огляд ресурсів, перераховані нижче, щоб вирішити проблему, ваш тепер.</span><span class="sxs-lookup"><span data-stu-id="d6929-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="d6929-104">Деякі загальні питання і резолюції кроки:</span><span class="sxs-lookup"><span data-stu-id="d6929-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="d6929-105">**Пристрої не зашифровані помилка на порталі компанії:** Новіші версії Android, особливо починаючи з v 7.0, вимагають запуску ввести пароль, щоб переконатися, що ваш пристрій повністю шифрується.</span><span class="sxs-lookup"><span data-stu-id="d6929-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="d6929-106">Спільні рішення, щоб увімкнути автозавантаження PIN-код або повністю зашифрувати пристрою.</span><span class="sxs-lookup"><span data-stu-id="d6929-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="d6929-107">Огляд [цей документ](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) для отримання додаткової інформації.</span><span class="sxs-lookup"><span data-stu-id="d6929-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="d6929-108">**Пристрої не заглядати Intune служби або відобразити як "Нездорових" в консолі адміністратора Intune:** Деякі Samsung 4.4 і 5,5 пристроїв не можуть перевірити на службу.</span><span class="sxs-lookup"><span data-stu-id="d6929-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="d6929-109">Існує 3 можливих рішень цієї проблеми:</span><span class="sxs-lookup"><span data-stu-id="d6929-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="d6929-110">Вручну відкрити портал компанії Intune програма, яка буде автоматично ініціювати пристрій синхронізації.</span><span class="sxs-lookup"><span data-stu-id="d6929-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="d6929-111">Оновити пристрій Android 6.0 або вище.</span><span class="sxs-lookup"><span data-stu-id="d6929-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="d6929-112">Вимкнути Samsung смарт-менеджер з управління портал компанії Intune.</span><span class="sxs-lookup"><span data-stu-id="d6929-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="d6929-113">Огляд [цей документ](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) для більш докладної інформації з цих питань і резолюцій.</span><span class="sxs-lookup"><span data-stu-id="d6929-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="d6929-114">**Користувача ліцензії типу неприпустимий** або **користувач ім'я не розпізнано помилка:** що користувачеві необхідно призначити Intune або EMS ліцензії.</span><span class="sxs-lookup"><span data-stu-id="d6929-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="d6929-115">Перегляньте ці документи до призначите ліцензію через: офіс центру адміністрування або Azure порталу.</span><span class="sxs-lookup"><span data-stu-id="d6929-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="d6929-116">Додаткові ресурси, щоб допомогти вирішити вашу проблему:</span><span class="sxs-lookup"><span data-stu-id="d6929-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="d6929-117">Використовувати [Intune виправлення неполадок портал](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) діагностувати та усунути поширені зарахування невдач.</span><span class="sxs-lookup"><span data-stu-id="d6929-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="d6929-118">Огляд [цей документ](https://docs.microsoft.com/intune/help-desk-operators) для більш докладної інформації.</span><span class="sxs-lookup"><span data-stu-id="d6929-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="d6929-119">Огляд [цей документ](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) список поширених помилок, які заважають заявки на участь та постанов до кожного.</span><span class="sxs-lookup"><span data-stu-id="d6929-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="d6929-120">[Дізнайтеся, як записатися Android пристроїв у Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="d6929-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
