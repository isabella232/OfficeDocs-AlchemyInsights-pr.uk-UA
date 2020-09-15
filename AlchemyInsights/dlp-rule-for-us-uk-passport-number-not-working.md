---
title: Правило DLP для паспорта США або Великобританії не працює
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679245"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Проблеми з номерами паспорта DLP-US/UK

**Важливо**: у ці безпрецедентні часи ми докладаємо всіх зусиль до того, щоб служби SharePoint Online і OneDrive були завжди доступні. Докладні відомості надано у статті [Тимчасові коригування функцій SharePoint Online](https://aka.ms/ODSPAdjustments).

**Помилки DLP із паспортами US/UK**

У вас виникли проблеми з **запобіганням втрати даних (DLP)** , які не працюють для вмісту, що містить **паспорт ГРОМАДЯНИНА США або Великобританії** , коли використовується тип конфіденційної інформації DLP у O365? Якщо це так, переконайтеся, що вміст містить потрібні відомості про те, що таке політика DLP шукає, коли вона обчислюється.
  
Наприклад, для паспорта " **номер для США/uk** ", настроєного на рівень впевненості в 75%, наведені нижче оцінки та мають виявлятися для показу правила.
  
- **[Формат:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Дев'ять цифр

- **[Візерунок:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Дев'ять послідовних цифр

- **[Контрольна сума:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ні, немає контрольної суми

- **[Визначення:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Політика DLP – 75% упевнений, що це тип конфіденційної інформації, якщо в безпосередній близькості від 300 символів:

  - Функція Func_usa_uk_passport знаходить вміст, який відповідає шаблону.

  - Виявлено ключове слово з Keyword_passport.

    Наприклад, наведений нижче зразок буде тригер для **паспорта US/UK** : номер паспорта США 123456789

Щоб отримати докладні відомості про те, що потрібно знайти номер паспорта США або Великобританії для вашого вмісту, ознайомтеся з цим розділом у цій статті: [що таке типи конфіденційних даних, які шукають номер ПАСПОРТА США або Великобританії](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number) .
  
Використовуючи інший вбудований тип конфіденційної інформації, ознайомтеся з наведена нижче стаття для отримання відомостей про те, що необхідно для інших типів: [які типи важливих відомостей відображаються](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  