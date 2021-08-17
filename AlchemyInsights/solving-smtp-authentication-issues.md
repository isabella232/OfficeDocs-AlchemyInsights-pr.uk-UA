---
title: Увімкнення автентифікації SMTP та виправлення неполадок
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: d16389ca577970deaf743255f75dc86134e79dcab2fff8c33987532fc7ee1105
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890455"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>Увімкнення автентифікації SMTP та виправлення неполадок

Якщо потрібно активувати автентифікацію SMTP для поштової скриньки або ви отримуєте "Клієнт не автентифіковано", Помилка "Автентифікація невдала" або "SmtpClientAuthentication" з кодом 5.7.57 або 5.7.3 або 5.7.139 під час спроби надіслати повідомлення електронної пошти, автентифікацію пристрою або програми за допомогою Microsoft 365, щоб вирішити цю проблему, виконайте такі три дії:

1. [Вимкніть стандартні параметри безпеки Azure,](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) установлювши перемикач **Увімкнути стандартні параметри безпеки** в значення **Ні.**

    a. Увійдіть на портал Azure як адміністратор безпеки, адміністратор умовного доступу або глобальний адміністратор.<BR/>
    b. Перейдіть до Azure Active Directory > **Властивості.**<BR/>
    c. Виберіть **Елемент Керування параметрами безпеки за замовчуванням**.<BR/>
    d. Установіть для **параметра Увімкнути безпеку за замовчуванням значення** **Ні**.<BR/>
    e. Натисніть **кнопку Зберегти**.

2. [Увімкніть надсилання SMTP клієнта](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) в ліцензованій поштовій скриньці.

    a. У Центр адміністрування Microsoft 365 перейдіть до **пункту Активні** користувачі та виберіть користувача.<BR/>
    b. Перейдіть на вкладку Пошта та в розділі Програми **електронної пошти** виберіть керування **програмами електронної пошти**.<BR/>
    d. **Переконайтеся, що прапорець Автентифікований SMTP** (увімкнуто).<BR/>
    e. Виберіть **Save changes (Зберегти зміни).**<BR/>

3. [Вимкніть багатофакторну автентифікацію (MFA)](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) у ліцензованій поштовій скриньці.

    a. Перейдіть до меню Центр адміністрування Microsoft 365 в меню переходів ліворуч виберіть **Активні**  >  **користувачі.**<BR/>
    b. Виберіть **Багатофакторна автентифікація.**<BR/>
    c. Виберіть користувача та **вимкніть multi-Factor auth.**<BR/>
