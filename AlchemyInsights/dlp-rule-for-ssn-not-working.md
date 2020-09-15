---
title: Правило DLP для SSN не працює
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679390"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Помилки DLP із номерами соціального страхування

**Важливо**: у ці безпрецедентні часи ми докладаємо всіх зусиль до того, щоб служби SharePoint Online і OneDrive були завжди доступні. Докладні відомості надано у статті [Тимчасові коригування функцій SharePoint Online](https://aka.ms/ODSPAdjustments).

**Проблеми з DLP, які містять SSNs**

У вас виникли проблеми з **запобіганням втрати даних (DLP)** , які не працюють для вмісту, що містить **номер соціального страхування (SSN)** під час використання типу конфіденційної інформації в Microsoft 365? Якщо це так, переконайтеся, що вміст містить потрібні відомості про те, що таке політика DLP шукає. 
  
Наприклад, для політики SSN, настроєного на рівень впевненості в 85%, наведені нижче оцінки та мають виявлятися для запуску правила.
  
- **[Формат:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 цифр, які можуть перебувати в форматованому або неформатований шаблоні

- **[Візерунок:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Чотири функції шукають SSNs в чотирьох різних шаблонах:

  - Func_ssn знаходить SSNs з попередньо 2011 сильним форматуванням, відформатованими з тире або пробілами (DDD-DD-DDDD або DD DD DDDD)

  - Func_unformatted_ssn знаходить SSNs з попередньо 2011 сильним форматуванням, які не відформатовано як дев'ять послідовних цифр (ddddddddd)

  - Func_randomized_formatted_ssn знаходить пост-2011 SSNs, відформатовані за допомогою тире або пробілів (DDD-DD-DDDD або DD DD DDDD)

  - Func_randomized_unformatted_ssn знаходить пост-2011 SSNs, які не форматовані як дев'ять послідовних цифр (ddddddddd)

- **[Контрольна сума:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Ні, немає контрольної суми

- **[Визначення:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Політика DLP – 85% упевнений, що це тип конфіденційної інформації, якщо в безпосередній близькості від 300 символів:

  - [Функція Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) знаходить вміст, який відповідає шаблону.

  - Виявлено ключове слово з [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) . Приклади ключових слів:  *Соціальна безпека, соціальне забезпечення #, SOC SEC, SSN*  . Наприклад, наведений нижче зразок буде тригер для політики DLP SSN: **SSN: 489-36-8350**
  
Щоб отримати докладні відомості про те, що потрібно для SSNs, які потрібно виявити для вашого вмісту, ознайомтеся з цим розділом у цій статті: [які типи конфіденційних даних шукають SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Використовуючи інший вбудований тип конфіденційної інформації, ознайомтеся з наведена нижче стаття для отримання відомостей про те, що необхідно для інших типів: [які типи важливих відомостей відображаються](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  