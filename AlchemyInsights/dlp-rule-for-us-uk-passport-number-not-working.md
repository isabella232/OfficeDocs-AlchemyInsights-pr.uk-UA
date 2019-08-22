---
title: DLP правило для США / Великобританія номер паспорта, не працює
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: bc91af8be58d49204f84cd7d22f481348af3c013
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529940"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Проблеми з DLP - США / Великобританія паспорт чисел

Виникають проблеми з **Запобігання втрати даних (DLP)** не працює для вмісту, який містить у **США / Великобританія номер паспорта** при використанні DLP конфіденційної інформації типу в O365? Якщо це так, переконайтеся, що ваш зміст містить необхідну інформацію для що DLP політики шукає коли його оцінка.
  
Наприклад, у **США / номер паспорта Великобританії** політику настроєно з рівня довіри до 75%, наступні оцінюються і повинні бути виявлені правило викликати
  
- **[Формат:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Дев'яти цифр

- **[Моделі:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Дев'ять послідовних цифр

- **[Контрольна сума:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ні, немає не контрольної суми

- **[Визначення:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP політика – 75% впевнені, що вона виявила цей тип конфіденційну інформацію if, в безпосередній близькості від 300 символів:

  - Функція Func_usa_uk_passport знаходить вміст, який відповідає візерунку.

  - Ключове слово з Keyword_passport знайшов.

    Наприклад, у наведеному прикладі ініціює для в **США / номер паспорта Великобританії** політики: номер паспорта США 123456789

Для отримання додаткової інформації про те, що потрібно для США / Великобританія номер паспорта, щоб бути виявлені для вашого змісту, дивіться наступний розділ у цій статті: [шукати те, що конфіденційних відомостей, надання яких США / номер паспорта Великобританії](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
За допомогою різних вбудований конфіденційної інформації типу, див. відомості про те, що вимагається для інших типів: [що конфіденційних відомостей, надання яких шукати](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  