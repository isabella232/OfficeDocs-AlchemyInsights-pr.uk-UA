---
title: Використання умовного доступу з Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 23afea21668191093d612d68ca6e9ab2a844f4a14977631d33f4fd956fc3c4e7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005795"
---
# <a name="using-conditional-access-with-intune"></a>Використання умовного доступу з Intune

Щоб використовувати умовний доступ з Intune, потрібно виконати 3 кроки:

- [Створіть політику відповідності, щоб визначити параметри, які мають відповідати вимогам для пристрою. Наприклад, для цього на ньому має бути pin-код із принаймні шести цифр.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Створіть політику умовного доступу, яка визначає ресурси для захисту, а також умови, які мають бути виконані для доступу до цих ресурсів. Наприклад, доступ до корпоративної електронної пошти має відповідати пристрою.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Переконайтеся, що як політики відповідності, так і політики умовного доступу призначено для потрібних груп користувачів. Для цього може знадобитися створити певні групи користувачів Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Докладніше...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
