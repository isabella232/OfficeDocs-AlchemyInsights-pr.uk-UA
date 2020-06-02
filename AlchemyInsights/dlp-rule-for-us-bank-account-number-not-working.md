---
title: "\"ЗВД\" правило для номера банківського рахунку США не працює"
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: b032a7c80e8b387114aeda95c4f6af7e57225517
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507355"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>ЗВД питання з номерами банківських рахунків США

**Важливо**: у ці безпрецедентні часи ми докладаємо всіх зусиль до того, щоб служби SharePoint Online і OneDrive були завжди доступні. Докладні відомості надано у статті [Тимчасові коригування функцій SharePoint Online](https://aka.ms/ODSPAdjustments).

**ЗВД питання з номерами банківських рахунків США**

У вас виникли проблеми з **запобігання втрати даних (звд)** , не працює для вмісту, який містить **номер банківського рахунку в США** під час використання тип Звд конфіденційної інформації в O365? Якщо це так, переконайтеся, що вміст містить потрібну інформацію про те, що в політиці ЗВД шукає, коли його оцінено.
  
Наприклад, для **американського банківського рахунку** політику, настроєну довірчий рівень 85%, оцінюються і має бути виявлено для запуску правила:
  
- **[Формат:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 цифр

- **[Візерунок:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 послідовних цифр.

- **[Контрольна сума:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ні, немає контрольної суми

- **[Визначення:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** ЗВД політика 75% впевнений, що він виявлений цей тип конфіденційної інформації, якщо в безпосередній близькості від 300 символів:

  - Регулярний вираз Regex_usa_bank_account_number знаходить вміст, який відповідає шаблону

  - Знайдено ключове слово з Keyword_usa_Bank_Account.

    Наприклад, наведений нижче зразок може викликати для **американського банківського рахунку** політики: розрахунковий рахунок 78344011

Для отримання додаткової інформації про те, що потрібно для того, щоб **номер банківського рахунку США** був виявлений для вашого вмісту, перегляньте наступний розділ у цій статті: [які типи конфіденційної інформації Шукайте номер банківського рахунку США](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Використовуючи інший вбудований тип конфіденційної інформації, зверніться до такої статті, щоб отримати відомості про те, що потрібно для інших типів: [які типи конфіденційних даних шукають](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  