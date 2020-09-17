---
title: Усунення несправностей із реєстрацією DEP в Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d32afde-47ab-4b1e-a669-662e5dbdc213
ms.custom:
- "783"
- "6200002"
ms.openlocfilehash: 50aab6e1e3c0d74d2e305e0bdd47c92b3a27c79f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47797317"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a><span data-ttu-id="47968-102">Усунення несправностей із реєстрацією DEP в Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="47968-102">Troubleshoot issues with DEP enrollment in Microsoft Intune</span></span>

<span data-ttu-id="47968-103">Перегляньте наведені нижче ресурси, щоб вирішити проблему.</span><span class="sxs-lookup"><span data-stu-id="47968-103">Review the resources listed below to resolve your issue now.</span></span>
  
1. <span data-ttu-id="47968-104">Якщо для пристрою DEP не вдається зареєструвати та (багатофакторну автентифікацію), вимкніть службу МЗС.</span><span class="sxs-lookup"><span data-stu-id="47968-104">If DEP device is unable to enroll and MFA (Multi-Factor Authentication) is enabled, please disable MFA.</span></span> <span data-ttu-id="47968-105">Зараз МЗС не підтримується для реєстрації DEP</span><span class="sxs-lookup"><span data-stu-id="47968-105">Currently MFA is not supported for DEP enrollment</span></span>

2. <span data-ttu-id="47968-106">Використовуйте [портал виправлення неполадок](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , щоб діагностувати та усунути поширені помилки в реєстрації.</span><span class="sxs-lookup"><span data-stu-id="47968-106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="47968-107">Перегляньте [цей документ](https://docs.microsoft.com/intune/help-desk-operators) , щоб отримати докладні відомості.</span><span class="sxs-lookup"><span data-stu-id="47968-107">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

3. <span data-ttu-id="47968-108">Перегляньте ці документи для списку поширених помилок, які перешкоджають виконанню та резолюціям кожного з них: [посібник із виправлення неполадок](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) і [Виправлення неполадок, пов'язаних із документами](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="47968-108">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span></span>

4. <span data-ttu-id="47968-109">[Дізнайтеся про програму реєстрації пристроїв](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span><span class="sxs-lookup"><span data-stu-id="47968-109">[Learn about device enrollment program](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span></span>
