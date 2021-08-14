---
title: Правило DLP для номера банківського рахунку в США не працює
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
ms.openlocfilehash: d19b2dcc29e23fab522159945496165338a117a47bfcfcadf0b93e4e5f14464f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005039"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>Проблеми зі зв'язаними літерами банківських рахунків у США

**Важливо**: у ці безпрецедентні часи ми докладаємо всіх зусиль до того, щоб служби SharePoint Online і OneDrive були завжди доступні. Докладні відомості надано у статті [Тимчасові коригування функцій SharePoint Online](https://aka.ms/ODSPAdjustments).

**Проблеми зі зв'язаними літерами банківських рахунків у США**

Виникли проблеми із захистом від втрати даних **(DLP)** і не працюють у вмісті, який містить номер банківського рахунку в США, коли використовується тип даних, що містить відомості, що містяться в O365?  У такому разі переконайтеся, що вміст містить необхідні відомості про те, яку політику DLP шукає під час її оцінювання.
  
Наприклад, для  політики "Номери банківських рахунків" у США, настроєній із довірчим рівнем 85%, виявляється, що правило має активувати таке:
  
- **[Формат:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8–17 цифр

- **[Шаблон:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8–17 цифр поспіль.

- **[Контрольна перевірка:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ні, такої перевірки немає.

- **[Визначення.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Політика DLP з імовірсом 75% впевнена, що цей тип конфіденційної інформації виявлено, якщо в межах 300 символів:

  - Регулярний вираз Regex_usa_bank_account_number знаходить вміст, який відповідає шаблону.

  - Виявиться ключове Keyword_usa_Bank_Account зі списку.

    Наприклад, наведений нижче зразок тригера політики **"Номер** банківського рахунку" (США): Checking Account 78344011

Докладні відомості про те,  що потрібно для виявлення номера банківського рахунку в США, див. в розділі цієї статті: Як виглядає номер банківського рахунку в [США?](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Відомості про те, що потрібно для інших типів, див. в цій [статті.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  