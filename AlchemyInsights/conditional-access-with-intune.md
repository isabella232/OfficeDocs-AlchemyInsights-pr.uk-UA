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
# <a name="conditional-access-with-intune"></a>Умовний доступ з InTune

За допомогою **умовного доступу** з InTune потрібно 3 кроки:

- Створіть **політику відповідності** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [IOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) для визначення параметрів, які повинні бути виконані до того, як пристрій вважається сумісним. Наприклад, пристрій повинен мати PIN-код принаймні 6 цифр, перш ніж він вважатиметься сумісним.
- Створіть **політику умовного доступу** , яка визначає, які ресурси захищено, і які умови повинні бути виконані для доступу до цих ресурсів.  [Наприклад,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) пристрій має відповідати вимогам, перш ніж отримати доступ до корпоративної електронної пошти.
- Переконайтеся, що **політика відповідності** та **політика умовного доступу** орієнтовані на потрібних груп користувачів. Це може знадобитися, створення певних груп користувачів у Azure Active Directory.

**Корисні посилання:**

[Огляд відповідності пристрою](https://docs.microsoft.com/intune/device-compliance-get-started)

[Усунення несправностей CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Політика щодо виправлення неполадок](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

Для захисту електронної пошти (Exchange Online) від доступу до несумісних пристроїв, обидва документи повинні дотримуватися:

1. [Захист доступу до електронної пошти з пристроїв за допомогою EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Захистіть доступ до електронної пошти з пристроїв за допомогою сучасних автентифікації клієнтів, як Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)