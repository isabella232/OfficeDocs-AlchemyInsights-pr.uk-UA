---
title: Настроювання DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808728"
---
# <a name="setup-dkim"></a>Настроювання DKIM

У цій [статті наведено повні](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)вказівки з настроювання DKIM для користувацьких доменів у Microsoft 365.

1. Для **кожного** настроюваного домену потрібно створити **два** записи CNAME DKIM у службі розміщення DNS-доменів свого домену (зазвичай це реєстратор доменів). Наприклад, contoso.com і fourthcoffee.com вимагають чотири записи CNAME DKIM: два для contoso.com і два для fourthcoffee.com.

   Записи CNAME DKIM для **кожного** настроюваного домену використовують такі формати:

   - **Ім'я хоста**: `selector1._domainkey.<CustomDomain>`

     **Указує на адресу або значення**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Ім'я хоста**: `selector2._domainkey.<CustomDomain>`

     **Указує на адресу або значення**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> – це текст ліворуч `.mail.protection.outlook.com` у настроюваному ЗАПИСІ MX для настроюваного домену (наприклад, `contoso-com` для домену contoso.com). \<InitialDomain\> – домен, який ви використовували під час реєстрації в Microsoft 365 (наприклад, contoso.onmicrosoft.com).

2. Створивши записи CNAME для користувацьких доменів, виконайте наведені нижче вказівки.

   муніципалітет. [Увійдіть у службу Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) за допомогою робочого або навчального облікового запису.

   b. Виберіть піктограму запускача програм у лівому верхньому куті, а потім виберіть елемент **адміністратор**.

   c. У нижній лівій частині вкладки розгорніть розділ **адміністратор** і натисніть кнопку **Exchange**.

   d. Перейдіть на сторінку **захист**  >  **DKIM**.

   e. Виберіть домен, а потім натисніть кнопку **Увімкнути** , щоб **підписати повідомлення для цього ДОМЕНУ з підписами DKIM**. Повторіть цей крок для кожного настроюваного домену.
