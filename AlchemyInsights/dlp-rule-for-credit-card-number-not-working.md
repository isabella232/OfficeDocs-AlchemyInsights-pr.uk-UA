---
title: Правило DLP для номера кредитної картки не працює
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
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679462"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Проблеми з DLP з номерами кредитних карток

**Важливо**: у ці безпрецедентні часи ми докладаємо всіх зусиль до того, щоб служби SharePoint Online і OneDrive були завжди доступні. Докладні відомості надано у статті [Тимчасові коригування функцій SharePoint Online](https://aka.ms/ODSPAdjustments).

**Проблеми з DLP з номерами кредитних карток**

У вас виникли проблеми з **запобіганням втрати даних (DLP)** , які не працюють для вмісту, що містить **номер кредитної картки** , якщо використовується тип конфіденційної інформації DLP у O365? Якщо це так, переконайтеся, що вміст містить необхідну інформацію, щоб ініціювати політику DLP, коли її оцінено. Наприклад, для **політики кредитної картки** , настроєної на рівень впевненості в 85%, наведені нижче оцінки та мають виявлятися для показу правила.
  
- **[Формат:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 цифр, які можуть бути відформатовані або неформатовані (dddddddddddddddd) і повинні пройти тест Luhn.

- **[Візерунок:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Дуже складний і надійний візерунок, який виявляє картки з усіх основних брендів по всьому світу, зокрема Visa, MasterCard, Discover картки, JCB, American Express, подарункових карток і карток Diner.

- **[Контрольна сума:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Так, контрольна сума Luhn

- **[Визначення:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Політика DLP – 85% упевнений, що це тип конфіденційної інформації, якщо в безпосередній близькості від 300 символів:

  - Функція Func_credit_card знаходить вміст, який відповідає шаблону.

  - Один із наведених нижче варіантів має значення ІСТИНА.

  - Виявлено ключове слово з Keyword_cc_verification.

  - Знайдено ключове слово з Keyword_cc_name

  - Функція Func_expiration_date знаходить дату в правильному форматі дати.

  - Контрольна сума проходить

    Наприклад, наведений нижче зразок буде тригер для політики номера кредитної картки DLP:

  - Віза: 4485 3647 3952 7352
  
  - Термін дії: 2/2009

Щоб отримати докладні відомості про те, що потрібно знайти для вашого вмісту **номер кредитної картки** , ознайомтеся з такими розділами в цій статті: [що таке важливі типи даних, які шукають кредитну картку #](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Використовуючи інший вбудований тип конфіденційної інформації, ознайомтеся з наведена нижче стаття для отримання відомостей про те, що необхідно для інших типів: [які типи важливих відомостей відображаються](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  