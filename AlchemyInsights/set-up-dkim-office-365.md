---
title: Setup DKIM
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
ms.openlocfilehash: 5dc90965516cc4d360b9be56c7737c6d134123ea8ac263b092559dd1416faff4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54108577"
---
# <a name="setup-dkim"></a>Setup DKIM

Повні інструкції з настроювання DKIM для настроюваних доменів у Microsoft 365 [нижче.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

1. Для **кожного** настроюваного домену потрібно створити два записи **CNAME** DKIM у службі розміщення DNS домену (зазвичай це реєстратор доменів). Наприклад, contoso.com і fourthcoffee.com DKIM CNAME: два для contoso.com і два для fourthcoffee.com.

   Для записів CNAME DKIM **для кожного настроюваного** домену використовуються такі формати:

   - **Ім'я хоста:**`selector1._domainkey.<CustomDomain>`

     **Указує на адресу або значення:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL (TTL):** 3600

   - **Ім'я хоста:**`selector2._domainkey.<CustomDomain>`

     **Указує на адресу або значення:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL (TTL):** 3600

   \<DomainGUID\> – це текст ліворуч від настроюваного запису MX для настроюваного домену (наприклад, для домену `.mail.protection.outlook.com` `contoso-com` contoso.com). \<InitialDomain\>– домен, який використовувався під час реєстрації в Microsoft 365 (наприклад, contoso.onmicrosoft.com).

2. Створивши записи CNAME для настроюваних доменів, виконайте такі дії:

   a. [увійдіть в обліковий Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) за допомогою робочого або навчального облікового запису.

   b. Клацніть піктограму запускача програм у лівому верхньому куті, а потім виберіть **адміністратор**.

   c. У нижній лівій області переходів **розгорніть елемент** Адміністратор **і виберіть Exchange**.

   d. Відкрийте меню **Protection**  >  **DKIM (Захист DKIM).**

   e. Виберіть домен і натисніть кнопку Увімкнути **для** **підписування повідомлень для цього домену за допомогою підписів DKIM.** Повторіть цю дію для кожного настроюваного домену.
