---
title: DLP правило для нас номер банківського рахунку не працює
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 9ebfa6bc09cef9ab7c30bddb4fcb8b6be3ab55a5
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29916437"
---
Виникли проблеми із **Запобігання втрати даних (DLP)** не працює для вмісту, який містить **Номер банківського рахунку США** при використанні DLP конфіденційної інформації типу в O365? Якщо це так, переконайтеся, що ваш зміст містить необхідну інформацію для що DLP політики шукає коли його оцінка. 
  
Наприклад, для політики **США номер банківського рахунку** з рівня довіри до 85%, такі оцінюються і повинні бути виявлені правило викликати: 
  
- **[Формат:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 цифр 
    
- **[Моделі:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 послідовних цифр. 
    
- **[Контрольна сума:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ні, немає не контрольної суми 
    
- **[Визначення:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** DLP політика – 75% впевнені, що вона виявила цей тип конфіденційну інформацію if, в безпосередній близькості від 300 символів: 
    
  - Регулярний вираз Regex_usa_bank_account_number знаходить вміст, який відповідає візерунку
    
  - Ключове слово з Keyword_usa_Bank_Account знайшов.
    
    Наприклад, у наведеному прикладі ініціює політики **США номер банківського рахунку** : розрахунковий рахунок 78344011 
    
Більш докладну інформацію про те, що вимагається для **США номер банківського рахунку** , щоб бути виявлені за ваш контент у розділі нижче в цій статті: [Те, що чутливої інформації типи шукати номер банківського рахунку в США](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
За допомогою різних вбудований конфіденційної інформації типу, див. відомості про те, що вимагається для інших типів: [що конфіденційних відомостей, надання яких шукати](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

