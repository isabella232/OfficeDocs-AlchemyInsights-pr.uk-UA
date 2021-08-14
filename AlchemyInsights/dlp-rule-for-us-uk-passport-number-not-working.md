---
title: Правило DLP для коду паспорта США та Великої Британії та України не працює
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
ms.openlocfilehash: 85e3ed7fdc221981de13ab6e2ada8adf2a3a80b40ff163981e047cc4a02a1514
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004967"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Проблеми з DLP – номери паспортів у США та Великобританії

**Важливо**: у ці безпрецедентні часи ми докладаємо всіх зусиль до того, щоб служби SharePoint Online і OneDrive були завжди доступні. Докладні відомості надано у статті [Тимчасові коригування функцій SharePoint Online](https://aka.ms/ODSPAdjustments).

**Проблеми зі зв'язаними лікувальними зв'язаннями з кодами паспортів США та Великої Британії та Великої Британії та Сша**

Виникли проблеми із захистом від втрати даних **(DLP)** у вмісті, який містить код паспорта США або Великої Британії та Великої Британії букв, коли використовується тип захисту від втрати даних в O365?  У такому разі переконайтеся, що вміст містить необхідні відомості про те, яку політику DLP шукає під час її оцінювання.
  
Наприклад, для  політики номерів паспорта у США та Великій Британії та Великої Британії та Сша, налаштованих із довірчим рівнем 75%, ми оцінюємо наведений нижче рівень і його потрібно визначити, щоб правило запускало
  
- **[Формат:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Дев'ять цифр

- **[Шаблон:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Дев'ять цифр без цифр

- **[Контрольна перевірка:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ні, такої перевірки немає.

- **[Визначення.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Політика DLP з імовірсом 75% впевнена, що цей тип конфіденційної інформації виявлено, якщо в межах 300 символів:

  - Функція Func_usa_uk_passport знаходить вміст, який відповідає шаблону.

  - Виявиться ключове Keyword_passport зі списку.

    Наприклад, наведений нижче зразок  тригера політиці чисть паспорта для США та Сполученого Сполученого Великої Британії та Герцогогі має номер паспорта: номер паспорта 123456789

Докладні відомості про те, що потрібно для виявлення номера паспорта для США та Великої Британії та Великої Британії та Сша, див. в розділі цієї статті: Як виглядає номер паспорта в США та [Великобританії.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Відомості про те, що потрібно для інших типів, див. в цій [статті.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  