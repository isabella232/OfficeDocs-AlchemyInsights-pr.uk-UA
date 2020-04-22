---
title: ЗВД правило для номера кредитної картки не працює
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 80ff41b3e746f95278ccbf0df19eebb61f7f9ee0
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704222"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>ЗВД питання з номерами кредитних карток

**Важливо**: у ці безпрецедентні часи ми докладаємо всіх зусиль до того, щоб служби SharePoint Online і OneDrive були завжди доступні. Докладні відомості надано у статті [Тимчасові коригування функцій SharePoint Online](https://aka.ms/ODSPAdjustments).

**ЗВД питання з номерами кредитних карток**

У вас виникли проблеми з **запобігання втрати даних (звд)** , не працює для вмісту, який містить **номер кредитної картки** під час використання тип інформації з конфіденційною звд в O365? Якщо так, переконайтеся, що вміст містить потрібну інформацію, щоб ініціювати політику ЗВД під час його обчислення. Наприклад, для **політики кредитної картки** , настроєної на довірчий рівень 85%, оцінюються і мають бути виявлені правила тригер:
  
- **[Формат:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 цифр, які можуть бути відформатовані або неформатований (ddddddddddddddddddddd) і повинні пройти тест Luhn.

- **[Візерунок:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Дуже складний і надійний шаблон, який виявляє карти з усіх основних брендів у всьому світі, включаючи Visa, MasterCard, Discover Card, JCB, American Express, подарункові картки, і закусочної карти.

- **[Контрольна сума:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Так, контрольна сума Luhn

- **[Визначення:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** ЗВД політика 85% впевнений, що він виявлений цей тип конфіденційної інформації, якщо в безпосередній близькості від 300 символів:

  - Функція Func_credit_card знаходить вміст, який відповідає шаблону.

  - Одна з таких дій істинна:

  - Знайдено ключове слово з Keyword_cc_verification.

  - Знайдено ключове слово з Keyword_cc_name

  - Функція Func_expiration_date знаходить дату в потрібному форматі дати.

  - Контрольна сума переходить

    Наприклад, наведений нижче зразок буде викликати на політику ЗВД кредитна картка номер:

  - Віза: 4485 3647 3952 7352
  
  - Термін дії: 2/2009

Для отримання додаткової інформації про те, що потрібно для того, щоб **номер кредитної картки** був виявлений для вашого вмісту, див у цьому розділі в цій статті: [які типи конфіденційної інформації Шукайте кредитну картку #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Використовуючи інший вбудований тип конфіденційної інформації, зверніться до такої статті, щоб отримати відомості про те, що потрібно для інших типів: [які типи конфіденційних даних шукають](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  