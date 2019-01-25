---
title: DLP правило для номер кредитної картки, не працює
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: a56f32b54e6cb32fa044d26d08868bac8c368de5
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/24/2019
ms.locfileid: "29496329"
---
Виникли проблеми із **Запобігання втрати даних (DLP)** не працює для вмісту, який містить **Номер кредитної картки** , при використанні DLP конфіденційної інформації типу в O365? Якщо це так, переконайтеся, що ваш зміст містить необхідну інформацію, щоб викликати в DLP політики, коли його оцінка. Наприклад, для **кредитних карт політики** з рівня довіри до 85%, такі оцінюються і повинні бути виявлені правило викликати: 
  
- **[Формат:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 цифр, яке можна форматувати або неформатований (dddddddddddddddd) і має пройти тест на Luhn. 
    
- **[Моделі:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Дуже складний і надійний зразок, який виявляє карт від всі основні бренди по всьому світу, включаючи Visa, Mastercard, Discover Card, JCB, American Express, подарункових карток і карток diner. 
    
- **[Контрольна сума:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Так, Luhn контрольної суми 
    
- **[Визначення:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP політика – 85% впевнені, що вона виявила цей тип конфіденційну інформацію if, в безпосередній близькості від 300 символів: 
    
  - Функція Func_credit_card знаходить вміст, який відповідає візерунку.
    
  - Одна з таких вірна: 
    
  - Ключове слово з Keyword_cc_verification знайшов.
    
  - Ключове слово з Keyword_cc_name знайдені
    
  - Функція Func_expiration_date знаходить дату у форматі дати правильний.
    
  - Контрольна сума проходить
    
    Наприклад, у наведеному прикладі ініціює DLP кредитної картки номер політики:
    
  - Віза: 4485 3647 3952 7352 
    
  - Термін дії: 2/2009
    
Більш докладну інформацію про те, що вимагається для **Номер кредитної картки** , щоб бути виявлені за ваш контент у розділі нижче в цій статті: [Те, що чутливої інформації типи шукати кредитної картки #](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
За допомогою різних вбудований конфіденційної інформації типу, див. відомості про те, що вимагається для інших типів: [що конфіденційних відомостей, надання яких шукати](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

