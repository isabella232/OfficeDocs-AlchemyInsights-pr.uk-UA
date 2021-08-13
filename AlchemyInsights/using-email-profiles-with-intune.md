---
title: Використання профілів електронної пошти в Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: b1653b73e7296e7eed411ae73c19342a1187b2eb7e287cff4339ea0ca32d75c1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919444"
---
# <a name="using-email-profiles-with-intune"></a>Використання профілів електронної пошти в Intune

За допомогою Intune можна створювати й розгортати профілі електронної пошти для вбудованого (вбудованого) клієнта електронної пошти на кількох платформах пристроїв.

Відомості про деякі обмеження, пов'язані з профілями електронної пошти, зокрема про те, як обробляються наявні профілі та як видалити профілі електронної пошти, див. в статті Додавання настройок електронної пошти до пристроїв за допомогою [Intune.](https://docs.microsoft.com/intune/email-settings-configure)

Докладні відомості про створення профілів електронної пошти для кожної платформи пристроїв див. в таких статтях:

[Параметри пристрою Android для настроювання електронної пошти, автентифікації та синхронізації в Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Додавання настройок електронної пошти для пристроїв iOS і iPadOS Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Параметри профілю електронної пошти в Microsoft Intune для пристроїв із windows Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Параметри профілю електронної пошти для пристроїв, на Windows 10 в Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Поширена проблема синхронізації**

**KNOX на пристрої з Android запобігає синхронізації контактів, календаря та завдань із пристроями користувачів.**

У профілі електронної пошти KNOX для Android kNOX адміністратор може вирішити, які типи вмісту синхронізуються з пристроєм, увімкнувши кожен із них.

Якщо для будь-якого типу вмісту встановлено значення **Не** настроєно (за замовчуванням), цей тип вмісту не синхронізуватиться автоматично. Користувач може ввімкнути потрібний тип вмісту безпосередньо на пристрої вручну, але ця конфігурація перезаписується параметром політики Intune, а синхронізація припиняється для цього типу вмісту.

