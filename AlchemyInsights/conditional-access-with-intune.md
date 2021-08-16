---
title: Умовний доступ з Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c24451fba8b8ab8fe7a1778bb292dec6678e1ef487076d27458c9aeb4963c683
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069733"
---
# <a name="conditional-access-with-intune"></a>Умовний доступ з Intune

Щоб  **використовувати умовний доступ**  з Intune, потрібно виконати 3 кроки:

- Створіть **політику відповідності** [(Android,](https://docs.microsoft.com/intune/compliance-policy-create-android) [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios) [Windows),](https://docs.microsoft.com//intune/compliance-policy-create-windows)щоб визначити параметри, які мають відповідати вимогам для пристрою. Наприклад, для цього на ньому має бути pin-код із принаймні шести цифр.
- Створіть **політику умовного доступу,**  яка визначає ресурси для захисту, а також умови, які мають бути виконані для доступу до цих ресурсів.  [Наприклад, доступ](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  до корпоративної електронної пошти має відповідати пристрою.
- **Переконайтеся, що як політики відповідності,** так і політики умовного доступу призначено для потрібних груп користувачів.  Для цього може знадобитися створити певні групи користувачів Azure Active Directory.

**Корисні посилання:**

[Огляд відповідності пристрою](https://docs.microsoft.com/intune/device-compliance-get-started)

[Виправлення неполадок, пов'язаних із центром спільного редагування](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Виправлення неполадок із політикою](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Щоб захистити електронну пошту (Exchange в Інтернеті) від доступу на несуповні пристрої, слід дотримуватися обох документів:

1. [Захист доступу до електронної пошти з пристроїв за допомогою служби EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Захистіть доступ до електронної пошти від пристроїв, використовуючи такі клієнти сучасної автентифікації, як Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)