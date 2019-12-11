---
title: Розгортання Office 365 ProPlus для спільного використання на RDS, сервер терміналів або VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959480"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a>Розгортання Office 365 ProPlus для спільного використання на RDS, сервер терміналів або VDI

Розгортання Office 365 ProPlus за допомогою служб віддалених робочих столів (RDS), раніше іменований служби терміналів:
- Потрібно мати Microsoft 365 бізнес-план або Office 365 план, який містить Office 365 ProPlus, наприклад Office 365 Enterprise E3 або Enterprise E5.
   > [!NOTE] 
   > Офіс 365 бізнес і офіс 365 бізнес преміум плани не включають в себе офіс 365 ProPlus.
- Потрібно ввімкнути [активацію спільної комп'ютера](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

> [!NOTE]
> Ви також можете завантажити та запустити [помічник з підтримки Microsoft і відновлення](https://aka.ms/SaRA_OfficeSCA_M365Portal) , щоб інсталювати Office 365 proplus у режим активації на спільному комп'ютері.

Щоб отримати додаткові відомості про передумови, інструкції з інсталяції та вказівки щодо настроюваних інсталяцій за допомогою засобу розгортання Office, див. [розгортання Office 365 ProPlus за допомогою служб віддалених робочих столів](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).

Щоб виправити помилки, пов'язані з активацією спільних комп'ютерів:
- Переглянути [вирішення проблем із активацією спільних комп'ютерів для Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- Див [скидання до стану активації Office 365 ProPlus](https://go.microsoft.com/fwlink/?linkid=2109218).

Якщо потрібно інсталювати Office 365 ProPlus на RDS з центру адміністрування Microsoft 365, ***який використовує параметри інсталяції за промовчанням***, виконайте такі дії:

1.  Перевірте, який план Office 365 у вас є. [Дізнатися як](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.  У разі потреби переключіться на інший план Office 365. [Дізнатися як](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.  Якщо Office вже інстальовано на сервері RDS, використовуючи будь-які інші плани Office 365, видаліть його. Наприклад, перейшовши на **панель** > керування,**видаліть програму**. Якщо ви працюєте з проблемами, видаліть за допомогою [служби підтримки Microsoft і помічника з відновлення](https://aka.ms/SARA-OfficeUninstall-Alchemy) .
4.  На сервері RDS ввійдіть до центру адміністрування Microsoft 365 за допомогою облікового запису адміністратора та [інсталюйте Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
5.  Після інсталяції Office ***не відкривайте або не входити в*** будь-які застосунки Office.
6.  На сервері RDS Увімкніть спільна Активація комп'ютера за допомогою редагування реєстру, виконавши такі дії:
   1. Клацніть правою кнопкою миші кнопку Windows у нижньому лівому куті екрана та виберіть пункт **виконати**. У полі "Відкрити" введіть **Regedit**і виберіть **"OK"**.
   2. Виберіть **так** , коли буде запропоновано дозволити редактору реєстру вносити зміни до пристрою.
   3. У редакторі реєстру, додайте значення рядка **Sharedcomputer ліцензування** з настройки 1 у розділі HKEY_LOCAL_MACHINE \ програмне забезпеченя \ Microsoft \Office\ClickToRun\Configuration.
   4. На сервері RDS ***ввійдіть як кінцевий користувач*** і [Переконайтеся, що активація спільного комп'ютера увімкнуто для Office 365 proplus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

