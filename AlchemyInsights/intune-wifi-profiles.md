---
title: InTune профілі Wi-Fi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555818"
---
# <a name="intune-wi-fi-profiles"></a>InTune профілі Wi-Fi

Успішне впровадження Wi-Fi підключення для клієнтів MDM залежить від правильно розгорнутого профілю, який відображає вимоги корпоративної інфраструктури Wi-Fi. Щоб переглянути відповідні параметри для клієнтських платформ, які ви розслідували, див.: 

[Додавання настройок Wi-Fi для пристроїв під керуванням ОС Android у Microsoft InTune](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Додавання параметрів Wi-Fi для Android Enterprise, присвячених і повністю керованих пристроїв у Microsoft InTune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[Додавання параметрів Wi-Fi для пристроїв iOS і Ipадос у Microsoft InTune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[Додавання настройок Wi-Fi для Windows 10 і пізніших пристроїв у InTune](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Імпорт параметрів Wi-Fi для пристроїв Windows у InTune](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**Поширених проблем**

**Я розгорнула профіль Wi-Fi, що залежить від розгорнутого сертифіката, вказаного в профілі Wi-Fi. Однак, профілі конфігурації відображаються стан помилки.**

Переконайтеся, що ваш пристрій отримав сертифікат.

1. У InTune перейдіть до **всіх пристроїв** і виберіть пристрій > **конфігурацію пристрою**.

2. Переконайтеся, що всі очікувані профілі перелічені та в успішному стані.

3. Для профілю Android, якщо у ланцюжку сертифікатів є проміжні сертифікати, переконайтеся, що вони розгорнуті на пристроях Android.

    Щоб перевірити стан сертифіката, перейдіть до **пристрою**  >  **профілі**конфігурації  >  **Android проміжні**  >  **Властивості**CA  >  **довірений сертифікат**.

Якщо ви продовжуєте бачити помилки, перегляньте розділи процедури та виправлення неполадок. Щоб отримати додаткові відомості див [Огляд для виправлення неполадок SCEP, профілі сертифікатів, з Microsoft InTune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).

**Я розгорнула профіль Wi-Fi на пристрій. InTune показує, що він був успішним, але пристрій не підключається до Wi-Fi.**

Успішний стан означає, що InTune успішно розгорнуто конфігурацію, як настроєно. Проте ці конфігурації можуть не відповідати вимогам для мережі та/або автентифікації. Щоб отримати докладніші відомості про спробу підключення, перегляньте журнали в службі інфраструктури та автентифікації (на контролері точки доступу Wi-Fi і сервері NPS/радіус). Можливо, доведеться працювати з командою мережної інфраструктури або постачальником Wi-Fi сторонніх виробників, щоб збирати й рецензувати журнали.