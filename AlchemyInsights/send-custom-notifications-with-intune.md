---
title: Надсилання користувацьких сповіщень за допомогою InTune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886878"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Як надсилати користувацькі сповіщення користувачам керованих iOS та Android пристроїв

Настроювані сповіщення для InTune обробляються застосунок порталу компанії на пристрої користувача. Потім програма створює Push-сповіщення на цьому пристрої.

Нижче наведено передумови пристрою для підтримки отримання користувацьких сповіщень, а також для програми, щоб створити Push-сповіщення:

- Пристрій повинен мати програму порталу компанії, встановленої.  

- Пристрій повинен дозволяти програмі "портал компанії" надсилати Push-сповіщення. Коли програма інсталюється або оновлюється, він запропонує користувачу дозвіл на отримання сповіщень.

- На пристроях Android потрібно встановити сервіси Google Play.

- Пристрій має бути зареєстровано з InTune.

Докладніші відомості про надсилання повідомлення наведено в [документації до функції](https://docs.microsoft.com/intune/custom-notifications).
