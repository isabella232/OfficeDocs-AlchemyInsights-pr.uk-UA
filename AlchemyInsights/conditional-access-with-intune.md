---
title: Умовний доступ з InTune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931457"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="ab219-102">Умовний доступ з InTune</span><span class="sxs-lookup"><span data-stu-id="ab219-102">Conditional Access with Intune</span></span>

<span data-ttu-id="ab219-103">За допомогою **умовного доступу** з InTune потрібно 3 кроки:</span><span class="sxs-lookup"><span data-stu-id="ab219-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="ab219-104">Створіть **політику відповідності** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [IOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) для визначення параметрів, які повинні бути виконані до того, як пристрій вважається сумісним.</span><span class="sxs-lookup"><span data-stu-id="ab219-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="ab219-105">Наприклад, пристрій повинен мати PIN-код принаймні 6 цифр, перш ніж він вважатиметься сумісним.</span><span class="sxs-lookup"><span data-stu-id="ab219-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="ab219-106">Створіть **політику умовного доступу** , яка визначає, які ресурси захищено, і які умови повинні бути виконані для доступу до цих ресурсів.</span><span class="sxs-lookup"><span data-stu-id="ab219-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="ab219-107">[Наприклад,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) пристрій має відповідати вимогам, перш ніж отримати доступ до корпоративної електронної пошти.</span><span class="sxs-lookup"><span data-stu-id="ab219-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="ab219-108">Переконайтеся, що **політика відповідності** та **політика умовного доступу** орієнтовані на потрібних груп користувачів.</span><span class="sxs-lookup"><span data-stu-id="ab219-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="ab219-109">Це може знадобитися, створення певних груп користувачів у Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ab219-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="ab219-110">**Корисні посилання:**</span><span class="sxs-lookup"><span data-stu-id="ab219-110">**Helpful links:**</span></span>

[<span data-ttu-id="ab219-111">Огляд відповідності пристрою</span><span class="sxs-lookup"><span data-stu-id="ab219-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="ab219-112">Усунення несправностей CA</span><span class="sxs-lookup"><span data-stu-id="ab219-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="ab219-113">Політика щодо виправлення неполадок</span><span class="sxs-lookup"><span data-stu-id="ab219-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="ab219-114">Для захисту електронної пошти (Exchange Online) від доступу до несумісних пристроїв, обидва документи повинні дотримуватися:</span><span class="sxs-lookup"><span data-stu-id="ab219-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="ab219-115">Захист доступу до електронної пошти з пристроїв за допомогою EAS</span><span class="sxs-lookup"><span data-stu-id="ab219-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="ab219-116">Захистіть доступ до електронної пошти з пристроїв за допомогою сучасних автентифікації клієнтів, як Outlook</span><span class="sxs-lookup"><span data-stu-id="ab219-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)