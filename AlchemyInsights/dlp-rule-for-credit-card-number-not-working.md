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
ms.openlocfilehash: bd4f200233d5571fc7b01576038e7b3951a07716a7d5948005418d2896291ee5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005111"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Проблеми зі зв'язаними лімітами зв'язку з номерами кредитних карток

**Важливо**: у ці безпрецедентні часи ми докладаємо всіх зусиль до того, щоб служби SharePoint Online і OneDrive були завжди доступні. Докладні відомості надано у статті [Тимчасові коригування функцій SharePoint Online](https://aka.ms/ODSPAdjustments).

**Проблеми зі зв'язаними лімітами зв'язку з номерами кредитних карток**

Виникли проблеми із захистом від втрати даних **(DLP)** під час використання в O365 вмісту, який містить номер кредитної картки,  У такому разі переконайтеся, що вміст містить необхідні відомості, щоб ініціювати політику DLP під час її оцінювання. Наприклад, для  політики кредитної картки, налаштованої з довірчим рівнем 85%, виявляється, що правило має активувати таке:
  
- **[Формат:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 цифр, які можуть бути відформатовані або неформатовані (ц), які мають пройти тест Луна.

- **[Шаблон:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Дуже складний і надійний шаблон, який виявляє картки всіх основних брендів у всьому світі, зокрема Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.

- **[Контрольна перевірка:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Так, контрольна перевірка Луна

- **[Визначення.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Політика захисту від загроз 85% упевнена, що виявлено цей тип конфіденційної інформації, якщо в межах 300 символів:

  - Функція Func_credit_card знаходить вміст, який відповідає шаблону.

  - Істинний варіант:

  - Виявиться Keyword_cc_verification зі списку.

  - Виявиться ключове слово Keyword_cc_name зі списку

  - Функція, Func_expiration_date знайде дату в правильному форматі.

  - Контрольна перевірка проходить

    Наприклад, наведений нижче зразок тригера політики номерів кредитної картки DLP:

  - Visa: 4485-3647-3952-7352
  
  - Термін дії завершується: 02.02.09

Докладні відомості про те,  що потрібно для виявлення номера кредитної картки для вмісту, див. в розділі цієї статті Як виглядає кредитна [картка#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Відомості про те, що потрібно для інших типів, див. в цій [статті.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  