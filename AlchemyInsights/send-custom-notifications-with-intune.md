---
title: Надсилання спеціальних сповіщень за допомогою Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 58acaa29f9d0b066cc7be6f6ee57b1806d0e8812b194e20166b133b7715226a8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086185"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Надсилання спеціальних сповіщень користувачам керованих пристроїв iOS і Android

Користувацькі сповіщення для Intune обробляються Company Portal програми на пристрої користувача. Після цього програма створить push-сповіщення на цьому пристрої.

Нижче перелічено передумови для підтримки отримання спеціальних сповіщень, а також для програми для створення push-сповіщення.

- На пристрої має бути інстальовано Company Portal програму.  

- Пристрій повинен дозволити програмі Company Portal надсилати push-сповіщення. Коли програму буде інстальовано або оновлено, користувачу буде запропоновано дозволити сповіщення.

- На пристроях з Android має бути інстальовано служби Google Play Services.

- Пристрій потрібно використовувати в Intune.

Докладні відомості, зокрема про те, як надіслати повідомлення, див. в [документації про функції.](https://docs.microsoft.com/intune/custom-notifications)
