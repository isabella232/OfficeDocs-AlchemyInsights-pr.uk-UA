---
title: Правило DLP для номера банківського рахунку США не працює
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679317"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>Проблеми з DLP з номерами банківського рахунку США

**Важливо**: у ці безпрецедентні часи ми докладаємо всіх зусиль до того, щоб служби SharePoint Online і OneDrive були завжди доступні. Докладні відомості надано у статті [Тимчасові коригування функцій SharePoint Online](https://aka.ms/ODSPAdjustments).

**Проблеми з DLP з номерами банківського рахунку США**

У вас виникли проблеми з **запобіганням втрати даних (DLP)** , які не працюють для вмісту, який містить **номер банківського рахунку США** , коли використовується тип конфіденційної інформації DLP у O365? Якщо це так, переконайтеся, що вміст містить потрібні відомості про те, що таке політика DLP шукає, коли вона обчислюється.
  
Наприклад, для політики **банківського рахунку США** , настроєного на рівень впевненості в 85%, наведені нижче оцінки та мають виявлятися для запуску правила.
  
- **[Формат:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 цифр

- **[Візерунок:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 послідовних цифр.

- **[Контрольна сума:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ні, немає контрольної суми

- **[Визначення:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Політика DLP – 75% упевнений, що це тип конфіденційної інформації, якщо в безпосередній близькості від 300 символів:

  - Регулярний вираз Regex_usa_bank_account_number знаходить вміст, який відповідає шаблону

  - Виявлено ключове слово з Keyword_usa_Bank_Account.

    Наприклад, наведений нижче зразок буде тригер для політики **банківського рахунку США** : перевірка облікового запису 78344011

Щоб отримати докладні відомості про те, що потрібно знайти **номер облікового запису банківського рахунку США** для вашого вмісту, ознайомтеся з цим розділом у цій статті: [які типи конфіденційних даних шукають номер банківського рахунку США](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Використовуючи інший вбудований тип конфіденційної інформації, ознайомтеся з наведена нижче стаття для отримання відомостей про те, що необхідно для інших типів: [які типи важливих відомостей відображаються](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  