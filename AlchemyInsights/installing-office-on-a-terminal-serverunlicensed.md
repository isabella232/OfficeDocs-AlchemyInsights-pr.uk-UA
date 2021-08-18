---
title: Інсталяція Office на сервері терміналів –неліцензований
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
ms.openlocfilehash: 35ef317ea87fedd01c08fee5b370e3c81e515c27
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58322020"
---
# <a name="installing-office-on-a-terminal-server"></a>Інсталяція Office на сервері терміналів

Щоб розгорнути Програми Microsoft 365 для підприємств на сервері Windows за допомогою служб віддалених робочих столів (RDS), раніше назвених служб терміналів:
  
- У вас має бути передплата Microsoft 365 що включає Програми Microsoft 365 для підприємств, наприклад Office 365 для підприємств E3 або "для підприємств E5". До Програми Microsoft 365 для бізнесу планів Програми Microsoft 365 для бізнесу Premium не входять Програми Microsoft 365 для підприємств.

- Потрібно ввімкнути активацію [на спільному комп'ютері.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

Якщо потрібно інсталювати пакет Програми Microsoft 365 для підприємств RDS із ***Центр адміністрування Microsoft 365,*** у якому використовуються настройки інсталяції за замовчуванням, виконайте наведені нижче дії.

    **Tip**: You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.
  
1. Перевірте, Microsoft 365 у вас є передплата. [Дізнайтеся, як](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. За потреби змініть передплату на іншу Microsoft 365 передплату. [Дізнайтеся, як](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Якщо Office RDS-сервер за допомогою будь-яких інших Microsoft 365 передплат, видаліть його. Наприклад, за допомогою панелі керування \> Видаліть програму. Видаліть за [допомогою Помічник із підтримки й відновлення](https://aka.ms/SARA-OfficeUninstall-Alchemy) Microsoft, якщо у вас виникають проблеми.

4. На сервері RDS увійдіть у свій обліковий Центр адміністрування Microsoft 365 та інсталюйте [Програми Microsoft 365 для підприємств](https://portal.office.com/OLS/MySoftware.aspx).

5. Після Office програми ***не*** відкривайте програми та не входьте в Office входу.

6. На сервері RDS увімкніть активацію на спільному комп'ютері, змінивши реєстр, виконавши такі дії:

1. Клацніть правою кнопкою миші Windows в нижньому лівому куті екрана та виберіть команду Виконати. У полі Відкрити введіть **regedit** і натисніть кнопку OK.

2. Коли з'явиться відповідний запит, натисніть кнопку Так, щоб дозволити редактор реєстру вносити зміни на пристрої.

3. У редакторі реєстру додайте значення рядка **SharedComputerLicensing** із значенням 1 у розділі HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. На сервері RDS увійдіть як користувач і переконайтеся, що активацію на спільному комп'ютері [Програми Microsoft 365 для підприємств.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded) 

Докладні відомості про попередні вимоги, інструкції з настроювання та вказівки з інсталяції за допомогою засобу розгортання Office див. в статті Розгортання [Програми Microsoft 365 для підприємств](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)за допомогою служб віддалених робочих столів.
  
Відомості про виправлення помилок, пов'язаних з активацією на спільному комп'ютері, див. в статті Виправлення неполадок з активацією на спільному [Програми Microsoft 365 для підприємств.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
  