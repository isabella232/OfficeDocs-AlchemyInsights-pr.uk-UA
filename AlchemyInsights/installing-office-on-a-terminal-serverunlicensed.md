---
title: Інсталяція Office на сервері терміналів-ліцензовано
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 7252efdc0f55b8923e685ec89f9b3c63882aa6b0
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763238"
---
# <a name="installing-office-on-a-terminal-server"></a>Інсталяція Office на сервері терміналів

Розгортання Microsoft 365 програм для підприємств на сервері Windows за допомогою служб віддалених робочих столів (RDS), раніше ім'я служби терміналів:
  
- Потрібно мати передплату Microsoft 365, який містить програми Microsoft 365 для підприємств, наприклад Office 365 Enterprise E3 або Enterprise E5. Програми Microsoft 365 для бізнесу та Microsoft 365 застосунки для бізнес-преміум плани не містять Microsoft 365 застосунки для підприємств.

- Потрібно ввімкнути [активацію спільної комп'ютера](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

Якщо потрібно інсталювати програми Microsoft 365 для Enterprise на RDS з центру адміністрування Microsoft 365, ***який використовує параметри інсталяції за промовчанням***, виконайте такі дії.

> [!TIP]
> Також можна завантажити та запустити помічника з [підтримки та відновлення Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) , щоб інсталювати програми Microsoft 365 для підприємств у режимі активації на спільному комп'ютері.
  
1. Перевірте, що ви маєте підписку Microsoft 365. [Дізнайтеся, як](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. У разі потреби переключіться на іншу передплату Microsoft 365. [Дізнайтеся, як](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Якщо Office вже інстальовано на сервері RDS, використовуючи будь-які інші передплати Microsoft 365, видаліть його. Наприклад, перейшовши на панель \> керування, видаліть програму. Якщо ви працюєте з проблемами, видаліть за допомогою [служби підтримки Microsoft і помічника з відновлення](https://aka.ms/SARA-OfficeUninstall-Alchemy) .

4. На сервері RDS ввійдіть до центру адміністрування Microsoft 365 з обліковим записом адміністратора та [інсталюйте програми Microsoft 365 для підприємств](https://portal.office.com/OLS/MySoftware.aspx).

5. Після інсталяції Office ***не відкривайте або не входити в*** будь-які застосунки Office.

6. На сервері RDS Увімкніть спільна Активація комп'ютера за допомогою редагування реєстру, виконавши такі дії:

1. Клацніть правою кнопкою миші кнопку Windows у нижньому лівому куті екрана та виберіть пункт Виконати. У полі "Відкрити" введіть **Regedit**і виберіть "OK".

2. Виберіть так, коли буде запропоновано дозволити редактору реєстру вносити зміни до пристрою.

3. У редакторі реєстру, додайте значення рядка **Sharedcomputer ліцензування** з настройки 1 у розділі HKEY_LOCAL_MACHINE \ програмне забезпеченя \ Microsoft \Office\ClickToRun\Configuration.

7. На сервері RDS ***ввійдіть як кінцевий користувач*** і [Переконайтеся, що активація спільного комп'ютера увімкнуто для Microsoft 365 програм для підприємств](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

Щоб отримати додаткові відомості про попередні вимоги, інструкції з настроювання та вказівки щодо настроювання інсталяції за допомогою засобу розгортання Office, перегляньте [розгортання Microsoft 365 застосунки для підприємств за допомогою служб віддалених робочих столів](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Щоб виправити помилки, пов'язані з активацією спільних комп'ютерів, перегляньте [вирішення проблем із активацією спільних комп'ютерів для програм Microsoft 365 для підприємств](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  