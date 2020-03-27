---
title: ЗВД правило для SSN не працює
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 4ec0df9d4954a8c65f0c34188d285dd8cf44a4f2
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977327"
---
# <a name="dlp-issues-with-social-security-numbers"></a>ЗВД питання з номерами соціального страхування

**Важливо**: у ці безпрецедентні часи Ми вживаємо заходів, щоб гарантувати, що служби SharePoint Online та OneDrive залишаються доступними – будь ласка, відвідайте [тимчасові функції SharePoint Online](https://aka.ms/ODSPAdjustments) для отримання додаткових відомостей.

**ЗВД проблеми з SSNs**

У вас виникли проблеми з **запобігання втрати даних (звд)** не працює для вмісту, який містить **номер соціального страхування (SSN)** під час використання тип конфіденційної інформації в Office 365? Якщо це так, переконайтеся, що вміст містить потрібну інформацію про те, що виглядає політика ЗВД. 
  
Наприклад, для політики SSN, настроєної на довірчий рівень 85%, обчислюються такі і повинні бути виявлені правила для запуску:
  
- **[Формат:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 цифр, які можуть бути відформатовані або неформатованим візерунком

- **[Візерунок:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Чотири функції Шукайте SSNs в чотирьох різних моделей:

  - Func_ssn знаходить SSNs з попередньо 2011 стійке форматування, відформатовані дефіси або пробіли (DDD-DD-DDDD або DDD DD DDDD)

  - Func_unformatted_ssn знаходить SSNs з попередньо 2011 стійке форматування, неформатований як дев'ять цифр (ddddddddd)

  - Func_randomized_formatted_ssn знаходить Post-2011 SSNs, відформатовані за допомогою тире або пробілів (DDD-DD-DDDD або DDD DD DDDD)

  - Func_randomized_unformatted_ssn знаходить Post-2011 SSNs, які неформатовані як дев'ять цифр (ddddddddd)

- **[Контрольна сума:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Ні, немає контрольної суми

- **[Визначення:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** ЗВД політика 85% впевнений, що він виявлений цей тип конфіденційної інформації, якщо в безпосередній близькості від 300 символів:

  - [Функція Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) знаходить вміст, який відповідає шаблону.

  - Знайдено ключове слово з [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) . Приклади ключових слів включають: *соціальне забезпечення, соціальне забезпечення #, СНС, SSN* . Наприклад, наведений нижче зразок буде тригер за ЗВД SSN політики: **SSN: 489-36-8350**
  
Для отримання додаткових відомостей про те, що потрібно для виявлення SSNs для вашого вмісту, див у розділі нижче в цій статті: [які типи конфіденційної інформації Шукайте SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Використовуючи інший вбудований тип конфіденційної інформації, зверніться до такої статті, щоб отримати відомості про те, що потрібно для інших типів: [які типи конфіденційних даних шукають](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  