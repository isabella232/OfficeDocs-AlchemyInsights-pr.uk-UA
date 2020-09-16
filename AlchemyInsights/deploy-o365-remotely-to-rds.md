---
title: Розгортання програм Microsoft 365 для підприємств для спільного використання в RDS, сервері терміналів або VDI
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 22ded616e82b2e82023b55a1d3ca6251cfb71712
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745556"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Розгортання програм Microsoft 365 для підприємств для спільного використання в RDS, сервері терміналів або VDI

Розгортання програм Microsoft 365 для підприємств за допомогою служб віддалених робочих столів (RDS), які раніше назвали служби терміналів:
- Потрібно мати план Microsoft 365 для бізнесу або план Office 365, що включає програми Microsoft 365 для підприємств, наприклад Office 365 Enterprise E3 або Enterprise E5.
   > [!NOTE] 
   > Стандартні плани програми Microsoft 365 для бізнесу та Microsoft 365 Business Premium не містять програм Microsoft 365 для підприємств.
- Потрібно ввімкнути [активацію спільного комп'ютера](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Ви також можете завантажити та запустити [помічник із підтримки й відновлення Microsoft,](https://aka.ms/SaRA_OfficeSCA_M365Portal) щоб інсталювати програми Microsoft 365 для підприємств у режимі активації спільного комп'ютера.

Докладні відомості про попередні вимоги, інструкції з настроювання та вказівки з настроювання настроюваних інсталяцій за допомогою засобу розгортання Office наведено в статті [розгортання програм Microsoft 365 для підприємств за допомогою служб віддаленого робочого стола](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

Щоб виправити помилки, пов'язані з активацією спільного комп'ютера, виконайте наведені нижче дії.
- Дізнайтеся, як [усунути проблеми з активацією спільного комп'ютера для програм Microsoft 365 для підприємств](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Докладні відомості див. в статті [Скидання стану активації програми Microsoft 365 для підприємств](https://go.microsoft.com/fwlink/?linkid=2109218).

Якщо потрібно інсталювати програми Microsoft 365 для підприємств на RDS у центрі адміністрування Microsoft 365, ***який використовує стандартні параметри інсталяції***, виконайте наведені нижче дії.

1.    Перевірте свою абонентську плату. [Дізнайтеся, як це зробити](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2.    Якщо потрібно, перейдіть до іншої передплатою. [Дізнайтеся, як це зробити](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3.    Якщо пакет Office уже інстальовано на сервері RDS, використовуючи будь-які інші передплати Microsoft, видаліть його. Наприклад, вибравши **панель керування**,  >  **видаліть програму**. Ви можете видалити за допомогою [помічника з підтримки й відновлення Microsoft,](https://aka.ms/SARA-OfficeUninstall-Alchemy) якщо ви працюєте з проблемами.
4.    На сервері RDS Увійдіть у центр адміністрування Microsoft 365 за допомогою облікового запису адміністратора та [інсталюйте програми Microsoft 365 для підприємств](https://portal.office.com/OLS/MySoftware.aspx).
5.    Після інсталяції Office ***не відкривайте та не ввійдіть в*** будь-які програми Office.
6.    На сервері RDS Увімкніть активацію спільного комп'ютера, змінивши реєстр, виконавши наведені нижче дії.
   1. Клацніть правою кнопкою миші кнопку Windows у лівому нижньому куті екрана та виберіть команду **виконати**. У полі Відкрити введіть **Regedit**, а потім натисніть **кнопку OK**.
   2. Натисніть кнопку **так** , коли з'явиться запит на дозвіл редактор реєстру, щоб внести зміни до вашого пристрою.
   3. У редакторі реєстру додайте рядне значення для **Sharedcompuitліцензування** з параметром 1 в розділі HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. На сервері RDS ***увійдіть як кінцевий користувач*** і [Переконайтеся, що активовано функцію активації спільного комп'ютера для програм Microsoft 365 для підприємств](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

