---
title: Налаштування DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0acaed476dbd06bc933bf466f9bf6116413a44bb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509405"
---
# <a name="setup-dkim"></a>Налаштування DKIM

Повні інструкції з налаштування DKIM для користувацьких доменів у Microsoft 365 є [тут](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

1. Для **кожного** настроюваного домену потрібно створити **два** записи DKIM CNAME у службі розміщення DNS вашого домену (зазвичай реєстратор доменів). Наприклад, contoso.com і fourthcoffee.com потрібні чотири записи DKIM CNAME: два для contoso.com і два для fourthcoffee.com.

   Записи DKIM CNAME для **кожного** настроюваного домену використовують такі формати:

   - **Ім'я хоста**:`selector1._domainkey.<CustomDomain>`

     **Вказує на адресу або значення**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Ім'я хоста**:`selector2._domainkey.<CustomDomain>`

     **Вказує на адресу або значення**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\>це текст зліва від `.mail.protection.outlook.com` настроюваного ЗАПИСУ MX для настроюваного домену (наприклад, `contoso-com` для домену contoso.com). \<InitialDomain\>це домен, який використовувався під час підписування для Microsoft 365 (наприклад, contoso.onmicrosoft.com).

2. Після створення записів CNAME для настроюваних доменів виконайте наведені нижче вказівки.

   є. [увійдіть до Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) з робочим або навчальним обліковим записом.

   B. Виберіть піктограму запуску програми у верхньому лівому куті та виберіть **адміністратор**.

   C. У лівій частині навігації розгорніть **адміністратор** і виберіть **Exchange**.

   D. Перейти до **захисту**  >  **DKIM**.

   E. Виберіть домен, а потім виберіть **Увімкнути** для **підписування повідомлень для цього ДОМЕНУ з підписами DKIM**. Повторіть цей крок для кожного настроюваного домену.
