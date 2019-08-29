---
title: Установки DKIM у службі Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: dd908db6a4bc1739b3c1cff059387034d67e093d
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666285"
---
# <a name="setup-dkim-in-office-365"></a>Установки DKIM у службі Office 365

Повна інструкція з налаштування DKIM, настроюваних доменів у службі Office 365 використовуються [тут](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. Для **кожного** користувача домену вам потрібно створити **два** записи DKIM CNAME вашого домену службі розміщення DNS (зазвичай Реєстратор домену). Наприклад, contoso.com і fourthcoffee.com вимагає чотири записи DKIM CNAME: два на contoso.com і два для fourthcoffee.com.

   На DKIM записи CNAME для **кожного** користувача домену за допомогою таких форматів:

   - **Ім'я хоста**:`selector1._domainkey.<CustomDomain>`

     **Пункту до значення або адресу**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Ім'я хоста**:`selector2._domainkey.<CustomDomain>`

     **Пункту до значення або адресу**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> текст ліворуч від `.mail.protection.outlook.com` в замовний запис MX для користувача домену (наприклад, `contoso-com` для домен contoso.com). \<InitialDomain\> є домен, які використовувалися під час реєстрації в Office 365 (наприклад, contoso.onmicrosoft.com).

2. Після створення запису CNAME записів для настроюваних доменів, виконайте наступні інструкції.

   муніципалітет. [Увійдіть до Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) з облікового запису роботи чи школи.

   b. Виберіть launcher піктограму у верхньому лівому і вибрати **адміністратора**.

   c. У нижньому лівому навігації розширити **адміністратора** і виберіть **Exchange**.

   d. Перейдіть до **захисту** > **DKIM**.

   e. Виберіть домен а потім виберіть **Увімкнути** для **підписати повідомлення для цього домену з DKIM підписами**. Повторіть цей крок для кожного користувача домену.
