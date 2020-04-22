---
title: Розгортання Microsoft 365 застосунки для підприємств, для спільного використання на RDS, сервер терміналів або VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: ddd44d40e9430ee31b8b734450dde0defef229d7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704726"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Розгортання Microsoft 365 застосунки для підприємств, для спільного використання на RDS, сервер терміналів або VDI

Для розгортання Microsoft 365 програм для підприємств за допомогою служб віддалених робочих столів (RDS), раніше ім'я служби терміналів:
- Потрібно мати Microsoft 365 бізнес-план або Office 365 план, який містить Microsoft 365 застосунки для підприємств, наприклад Office 365 Enterprise E3 або Enterprise E5.
   > [!NOTE] 
   > Microsoft 365 програми для бізнесу та Microsoft 365 бізнес-преміум стандартні плани не містять Microsoft 365 застосунки для підприємств.
- Потрібно ввімкнути [активацію спільної комп'ютера](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

> [!NOTE]
> Також можна завантажити та запустити помічника з [підтримки та відновлення Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) , щоб інсталювати програми Microsoft 365 для підприємств у режимі активації на спільному комп'ютері.

Щоб отримати додаткові відомості про передумови, інструкції з інсталяції та рекомендації щодо настроюваних інсталяцій за допомогою засобу розгортання Office, див. [розгортання програм Microsoft 365 для підприємств за допомогою служб віддалених робочих столів](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).

Щоб виправити помилки, пов'язані з активацією спільних комп'ютерів:
- Переглянути [вирішення проблем із активацією спільних комп'ютерів для Microsoft 365 програм для підприємств](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- Докладні відомості див. в статті [Скидання стану активації програми Microsoft 365 для підприємств](https://go.microsoft.com/fwlink/?linkid=2109218).

Якщо потрібно інсталювати програми Microsoft 365 для підприємств на RDS з центру адміністрування Microsoft 365, ***який використовує параметри інсталяції за промовчанням***, виконайте такі дії:

1.    Перевірте, яку підписку ви маєте. [Дізнатися як](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.    Якщо потрібно, переключіться на іншу підписку. [Дізнатися як](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.    Якщо Office вже інстальовано на сервері RDS, використовуючи будь-які інші передплати Microsoft, видаліть його. Наприклад, перейшовши на **панель** > керування,**видаліть програму**. Якщо ви працюєте з проблемами, видаліть за допомогою [служби підтримки Microsoft і помічника з відновлення](https://aka.ms/SARA-OfficeUninstall-Alchemy) .
4.    На сервері RDS ввійдіть до центру адміністрування Microsoft 365 з обліковим записом адміністратора та [інсталюйте програми Microsoft 365 для підприємств](https://portal.office.com/OLS/MySoftware.aspx).
5.    Після інсталяції Office ***не відкривайте або не входити в*** будь-які застосунки Office.
6.    На сервері RDS Увімкніть спільна Активація комп'ютера за допомогою редагування реєстру, виконавши такі дії:
   1. Клацніть правою кнопкою миші кнопку Windows у нижньому лівому куті екрана та виберіть пункт **виконати**. У полі "Відкрити" введіть **Regedit**і виберіть **"OK"**.
   2. Виберіть **так** , коли буде запропоновано дозволити редактору реєстру вносити зміни до пристрою.
   3. У редакторі реєстру, додайте значення рядка **Sharedcomputer ліцензування** з настройки 1 у розділі HKEY_LOCAL_MACHINE \ програмне забезпеченя \ Microsoft \Office\ClickToRun\Configuration.
   4. На сервері RDS ***ввійдіть як кінцевий користувач*** і [Переконайтеся, що активація спільного комп'ютера увімкнуто для Microsoft 365 програм для підприємств](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

