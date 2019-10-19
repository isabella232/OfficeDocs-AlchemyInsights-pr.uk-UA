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
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/18/2019
ms.locfileid: "37205430"
---
# <a name="installing-office-on-a-terminal-server"></a>Інсталяція Office на сервері терміналів

Для розгортання Office 365 ProPlus на сервері Windows за допомогою служб віддалених робочих столів (RDS), раніше іменований служби терміналів:
  
- Потрібно мати Office 365 план, який включає в себе Office 365 ProPlus, наприклад Office 365 Enterprise E3 або Enterprise E5. Офіс 365 бізнес і офіс 365 бізнес преміум плани не включають в себе офіс 365 ProPlus.

- Потрібно ввімкнути [активацію спільної комп'ютера](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

Якщо потрібно інсталювати Office 365 ProPlus на RDS з центру адміністрування Microsoft 365, ***який використовує параметри інсталяції за промовчанням***, виконайте такі дії.

> [!TIP]
> Ви також можете завантажити та запустити [помічник з підтримки Microsoft і відновлення](https://aka.ms/SaRA_OfficeSCA_M365Portal) , щоб інсталювати Office 365 proplus у режим активації на спільному комп'ютері.
  
1. Перевірте, який план Office 365 у вас є. [Дізнайтеся, як](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. У разі потреби переключіться на інший план Office 365. [Дізнайтеся, як](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Якщо Office вже інстальовано на сервері RDS, використовуючи будь-які інші плани Office 365, видаліть його. Наприклад, перейшовши на панель \> керування, видаліть програму. Якщо ви працюєте з проблемами, видаліть за допомогою [служби підтримки Microsoft і помічника з відновлення](https://aka.ms/SARA-OfficeUninstall-Alchemy) .

4. На сервері RDS ввійдіть до центру адміністрування Microsoft 365 за допомогою облікового запису адміністратора та [інсталюйте Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).

5. Після інсталяції Office ***не відкривайте або не входити в*** будь-які застосунки Office.

6. На сервері RDS Увімкніть спільна Активація комп'ютера за допомогою редагування реєстру, виконавши такі дії:

1. Клацніть правою кнопкою миші кнопку Windows у нижньому лівому куті екрана та виберіть пункт Виконати. У полі "Відкрити" введіть **Regedit**і виберіть "OK".

2. Виберіть так, коли буде запропоновано дозволити редактору реєстру вносити зміни до пристрою.

3. У редакторі реєстру, додайте значення рядка **Sharedcomputer ліцензування** з настройки 1, під HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. На сервері RDS ***ввійдіть як кінцевий користувач*** і [Переконайтеся, що активація спільного комп'ютера увімкнуто для Office 365 proplus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

Щоб отримати додаткові відомості про попередні вимоги, інструкції з настроювання та вказівки щодо настроюваних інсталяцій за допомогою засобу розгортання Office, див. [розгортання Office 365 ProPlus за допомогою служб віддалених робочих столів](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Щоб виправити помилки, пов'язані з активацією спільних комп'ютерів, перегляньте [Виправлення неполадок, пов'язаних із активацією спільних комп'ютерів для Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  