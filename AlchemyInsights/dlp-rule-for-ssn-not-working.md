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
ms.openlocfilehash: 3f30998fb3bc4c5442e4e1541b87d88ecd7df6eef3a50e719fa5014eb86af39c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005003"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Проблеми зі зв'язаними лінею в соціальних мережах

**Важливо**: у ці безпрецедентні часи ми докладаємо всіх зусиль до того, щоб служби SharePoint Online і OneDrive були завжди доступні. Докладні відомості надано у статті [Тимчасові коригування функцій SharePoint Online](https://aka.ms/ODSPAdjustments).

**Проблеми з DLP у SSN**

Проблеми із захистом від втрати даних **(DLP)** не працюють для вмісту, який містить номер соціального безпеки **(SSN)** під час використання в програмі Microsoft 365? У такому разі переконайтеся, що вміст містить необхідні відомості про те, яку політику DLP потрібна. 
  
Наприклад, для політики SSN, настроєної з довірчим рівнем 85 %, виявляється, що правило має активувати таке:
  
- **[Формат:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 цифр за форматованим або неформатованим шаблоном

- **[Шаблон:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Пошук SSN чотирьох функцій виявляються в чотирьох різних шаблонах:

  - Func_ssn знаходить SSN із надійним форматуванням до 2011 року, відформатованих тире або пробілами (ц-ц-ц АБО ц), які видано до 2011 року.

  - Func_unformatted_ssn знайде SSN з надійним форматуванням до 2011 року, які неформатовано як дев'ять послідовних цифр (ццц),

  - Func_randomized_formatted_ssn знаходить SSN, відформатовані за допомогою тире або пробілів (ц-цц-цц-ц АБО ц), які видано після 2011 року.

  - Func_randomized_unformatted_ssn знайде SSN після 2011 року, які неформатовані дев'ять послідовних цифр (ццц),

- **[Контрольна перевірка:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Ні, такої перевірки немає.

- **[Визначення.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Політика захисту від загроз 85% упевнена, що виявлено цей тип конфіденційної інформації, якщо в межах 300 символів:

  - Функція [Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) знаходить вміст, який відповідає шаблону.

  - Виявиться [ключове Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) зі списку. Приклади ключових слів: *Social Security, Social Security#, Soc Sec ,SSN.* Наприклад, наведений нижче зразок тригера політики SSN **DLP: SSN: 489-36-8350**
  
Докладні відомості про те, що потрібно зробити, щоб SSN виявляв ваш вміст, див. в розділі цієї статті Під час пошуку [SSN](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Відомості про те, що потрібно для інших типів, див. в цій [статті.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  