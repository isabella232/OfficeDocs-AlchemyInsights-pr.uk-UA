---
title: Інсталяція пакета Office на сервері терміналів – неліцензований
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663138"
---
# <a name="installing-office-on-a-terminal-server"></a>Інсталяція пакета Office на сервері терміналів

Для розгортання програм Microsoft 365 для підприємств на сервері Windows Server за допомогою служб віддалених робочих столів (RDS), які раніше назвали служби терміналів:
  
- Потрібно мати передплатну програму Microsoft 365, яка включає програми Microsoft 365 для підприємств, наприклад Office 365 Enterprise E3 або Enterprise E5. У планах програми Microsoft 365 для бізнесу та програм Microsoft 365 для бізнесу Premium не включаються програми Microsoft 365 для підприємств.

- Потрібно ввімкнути [активацію спільного комп'ютера](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Якщо потрібно інсталювати програми Microsoft 365 для підприємств на RDS у центрі адміністрування Microsoft 365, у ***якому використовуються стандартні параметри інсталяції***, виконайте наведені нижче дії.

> [!TIP]
> Ви також можете завантажити та запустити [помічник із підтримки й відновлення Microsoft,](https://aka.ms/SaRA_OfficeSCA_M365Portal) щоб інсталювати програми Microsoft 365 для підприємств у режимі активації спільного комп'ютера.
  
1. Перевірте, що таке Передплата на Microsoft 365. [Дізнайтеся, як](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Якщо потрібно, перейдіть до іншої абонентської плати Microsoft 365. [Дізнайтеся, як](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Якщо пакет Office уже інстальовано на сервері RDS, використовуючи будь-які інші передплати Microsoft 365, видаліть його. Наприклад, вибравши панель керування, \> видаліть програму. Ви можете видалити за допомогою [помічника з підтримки й відновлення Microsoft,](https://aka.ms/SARA-OfficeUninstall-Alchemy) якщо ви працюєте з проблемами.

4. На сервері RDS Увійдіть у центр адміністрування Microsoft 365 за допомогою облікового запису адміністратора та [інсталюйте програми Microsoft 365 для підприємств](https://portal.office.com/OLS/MySoftware.aspx).

5. Після інсталяції Office ***не відкривайте та не ввійдіть в*** будь-які програми Office.

6. На сервері RDS Увімкніть активацію спільного комп'ютера, змінивши реєстр, виконавши наведені нижче дії.

1. Клацніть правою кнопкою миші кнопку Windows у лівому нижньому куті екрана, а потім виберіть команду виконати. У полі Відкрити введіть **Regedit**, а потім натисніть кнопку OK.

2. Натисніть кнопку Так, коли з'явиться запит на дозвіл редактор реєстру, щоб внести зміни до вашого пристрою.

3. У редакторі реєстру додайте рядне значення для **Sharedcompuitліцензування** з параметром 1 в розділі HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. На сервері RDS ***увійдіть як кінцевий користувач*** і [Переконайтеся, що активовано функцію активації спільного комп'ютера для програм Microsoft 365 для підприємств](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Докладні відомості про попередні вимоги, інструкції з настроювання та вказівки щодо настроюваних інсталяцій за допомогою засобу розгортання Office наведено в статті [розгортання програм Microsoft 365 для підприємств за допомогою служб віддаленого робочого стола](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Щоб виправити помилки, пов'язані з активацією на спільному комп'ютері, ознайомтеся [з проблемами усунення проблем із підключенням до спільного комп'ютера для програм Microsoft 365 для підприємств](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  