---
title: Надсилання користувацьких сповіщень на InTune
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
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720667"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Надсилання власних сповіщень користувачам керованих пристроїв із iOS і Android

Користувацькі сповіщення для Inune обробляються програмою "портал компанії" на пристрої користувача. Після цього програма створить сповіщення про Push-повідомлення на цьому пристрої.

Нижче наведено попередні вимоги до пристрою, щоб підтримувати отримання власних сповіщень, а також для програми, щоб створити сповіщення про Push-повідомлення:

- На пристрої має бути інстальовано програму "портал компанії".  

- Пристрій має дозволити програмі "портал компанії" передавати Push-сповіщення. Коли програму інстальовано або оновлено, буде запропоновано користувачу дозволяти сповіщення.

- На пристроях з Android має бути інстальовано служби Google Play Services.

- Пристрій має бути зареєстровано в програмі Inune.

Щоб отримати докладні відомості, зокрема про те, як відправити повідомлення, ознайомтеся з [документацією для функцій](https://docs.microsoft.com/intune/custom-notifications).
