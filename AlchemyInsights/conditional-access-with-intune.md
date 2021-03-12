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
ms.openlocfilehash: 20ef8205431aad821419f2559be3402c8228d838
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704807"
---
# <a name="conditional-access-with-intune"></a>Умовний доступ за допомогою веб-програми Inune

Використання  **умовного доступу**  за допомогою функції inune вимагає 3 кроків:

- Створіть  **політику відповідності**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [IOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)), щоб визначити настройки, які потрібно виконати перед тим, як пристрій вважається сумісним. Наприклад, для пристрою має бути PIN-код принаймні на 6 цифр, перш ніж вона вважається відповідним.
- Створіть **політику умовного доступу**  , яка визначає, які ресурси захищено, і які умови потрібно виконати для доступу до цих ресурсів.  [Наприклад,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  пристрій має бути сумісним, перш ніж отримувати доступ до корпоративної електронної пошти.
- Переконайтеся, що **політики відповідності**  та  **політики умовного доступу**  орієнтовані на потрібні групи користувачів. Для цього може знадобитися створити певні групи користувачів у службі Azure Active Directory.

**Корисні посилання:**

[Огляд відповідності пристрою](https://docs.microsoft.com/intune/device-compliance-get-started)

[Виправлення неполадок із CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Виправлення неполадок із політикою](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Щоб захистити електронну пошту (Exchange Online) від програми Access за допомогою несумісних пристроїв, слід дотримуватися таких документів:

1. [Захист доступу до електронної пошти з пристроїв за допомогою EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Захист доступу до електронної пошти з пристроїв за допомогою сучасних клієнтів автентифікації, як-от Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)