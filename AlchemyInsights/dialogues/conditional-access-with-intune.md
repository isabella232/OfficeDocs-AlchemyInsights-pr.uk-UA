---
title: Використання умовного доступу за допомогою функції InTune
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
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694718"
---
# <a name="using-conditional-access-with-intune"></a>Використання умовного доступу за допомогою функції InTune

Використання умовного доступу за допомогою функції Inune вимагає 3 кроків:

- [Створіть політику відповідності, щоб визначити параметри, які потрібно виконати перед тим, як пристрій вважається сумісним. Наприклад, для пристрою має бути PIN-код принаймні на 6 цифр, перш ніж вона вважається відповідним.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Створіть політику умовного доступу, яка визначає, які ресурси захищено, і які умови потрібно виконати для доступу до цих ресурсів. Наприклад, пристрій має бути сумісним, перш ніж отримувати доступ до корпоративної електронної пошти.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Переконайтеся, що політики відповідності та політики умовного доступу орієнтовані на потрібні групи користувачів. Для цього може знадобитися створити певні групи користувачів у службі Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Докладніше...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
