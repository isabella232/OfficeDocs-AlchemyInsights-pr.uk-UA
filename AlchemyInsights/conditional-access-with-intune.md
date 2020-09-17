---
title: Умовний доступ за допомогою веб-програми Inune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807680"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="e1493-102">Умовний доступ за допомогою веб-програми Inune</span><span class="sxs-lookup"><span data-stu-id="e1493-102">Conditional Access with Intune</span></span>

<span data-ttu-id="e1493-103">Використання  **умовного доступу**  за допомогою функції inune вимагає 3 кроків:</span><span class="sxs-lookup"><span data-stu-id="e1493-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="e1493-104">Створіть  **політику відповідності**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [IOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)), щоб визначити настройки, які потрібно виконати перед тим, як пристрій вважається сумісним.</span><span class="sxs-lookup"><span data-stu-id="e1493-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="e1493-105">Наприклад, для пристрою має бути PIN-код принаймні на 6 цифр, перш ніж вона вважається відповідним.</span><span class="sxs-lookup"><span data-stu-id="e1493-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="e1493-106">Створіть **політику умовного доступу**  , яка визначає, які ресурси захищено, і які умови потрібно виконати для доступу до цих ресурсів.</span><span class="sxs-lookup"><span data-stu-id="e1493-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="e1493-107">[Наприклад,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  пристрій має бути сумісним, перш ніж отримувати доступ до корпоративної електронної пошти.</span><span class="sxs-lookup"><span data-stu-id="e1493-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="e1493-108">Переконайтеся, що **політики відповідності**  та  **політики умовного доступу**  орієнтовані на потрібні групи користувачів.</span><span class="sxs-lookup"><span data-stu-id="e1493-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="e1493-109">Для цього може знадобитися створити певні групи користувачів у службі Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e1493-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="e1493-110">**Корисні посилання:**</span><span class="sxs-lookup"><span data-stu-id="e1493-110">**Helpful links:**</span></span>

[<span data-ttu-id="e1493-111">Огляд відповідності пристрою</span><span class="sxs-lookup"><span data-stu-id="e1493-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="e1493-112">Виправлення неполадок із CA</span><span class="sxs-lookup"><span data-stu-id="e1493-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="e1493-113">Виправлення неполадок із політикою</span><span class="sxs-lookup"><span data-stu-id="e1493-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="e1493-114">Щоб захистити електронну пошту (Exchange Online) від програми Access за допомогою несумісних пристроїв, слід дотримуватися таких документів:</span><span class="sxs-lookup"><span data-stu-id="e1493-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="e1493-115">Захист доступу до електронної пошти з пристроїв за допомогою EAS</span><span class="sxs-lookup"><span data-stu-id="e1493-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="e1493-116">Захист доступу до електронної пошти з пристроїв за допомогою сучасних клієнтів автентифікації, як-от Outlook</span><span class="sxs-lookup"><span data-stu-id="e1493-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)