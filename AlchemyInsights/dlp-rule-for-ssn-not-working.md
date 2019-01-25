---
title: DLP правило для SSN не працює
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b92d122b774d97cd2e44cc0880dc5001065b57cc
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/24/2019
ms.locfileid: "29496366"
---
Вам мають проблеми з **Запобігання втрати даних (DLP)** не працює для вмісту, який містить **Номер соціального страхування Соціального страхування** при використанні конфіденційної інформації типу у службі Office 365 Якщо це так, переконайтеся, що ваш зміст містить необхідну інформацію за те, що політика DLP дивлячись. 
  
Наприклад, для SSN політику настроєно з рівня довіри до 85%, такі оцінюються і повинні бути виявлені правило викликати:
  
- **[Формат:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 цифр, які можуть бути в форматований або неформатований візерунком 
    
- **[Моделі:](https://msconnect.microsoft.com/https:/docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Чотири функції шукати SSNs в чотирьох різних моделей: 
    
  - Func_ssn знаходить SSNs з попередньо-2011 сильний форматування, відформатовані з тире або пробілів (ddd dd dddd OR ddd dd dddd)
    
  - Func_unformatted_ssn знаходить SSNs з попередньо-2011 сильний форматування, які не було відформатовано як дев'ять послідовні цифри (ddddddddd)
    
  - Func_randomized_formatted_ssn знаходить пост-2011 SSNs, які відформатовано з тире або пробілів (ddd dd dddd OR ddd dd dddd)
    
  - Func_randomized_unformatted_ssn знаходить пост-2011 SSNs, які є неформатований як дев'ять послідовні цифри (ddddddddd)
    
- **[Контрольна сума:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Ні, немає не контрольної суми 
    
- **[Визначення:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP політика – 85% впевнені, що вона виявила цей тип конфіденційну інформацію if, в безпосередній близькості від 300 символів: 
    
  - [Функція Func_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) знаходить вміст, який відповідає візерунку. 
    
  - Ключове слово з [Keyword_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) знайшов. Прикладами ключові слова: *соціальне забезпечення, соціальне забезпечення #, Soc сек, SSN* . Наприклад, у наведеному прикладі ініціює DLP SSN політики: **SSN: 36-489-8350**
    
Більш докладну інформацію про те, що вимагається для SSNs бути виявлені за ваш контент у розділі нижче в цій статті: [Те, що конфіденційних відомостей, надання яких шукати SSNs](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
За допомогою різних вбудований конфіденційної інформації типу, див. відомості про те, що вимагається для інших типів: [що конфіденційних відомостей, надання яких шукати](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

