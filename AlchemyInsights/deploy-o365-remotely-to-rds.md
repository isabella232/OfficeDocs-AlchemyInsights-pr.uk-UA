---
title: Розгортання Програми Microsoft 365 для підприємств для спільного використання в службах RDS, Термінал Server або VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 55b86557ec205dde2c459d76e8e330d2a8271dbec723f079e119ebe409b41c3f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031499"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Розгортання Програми Microsoft 365 для підприємств для спільного використання в службах RDS, Термінал Server або VDI

Щоб розгорнути Програми Microsoft 365 для підприємств служби віддалених робочих столів (RDS), раніше назвіть служби терміналів:

- У вас має бути план Microsoft 365 для бізнесу або план Office 365 який включає Програми Microsoft 365 для підприємств, наприклад Office 365 для підприємств E3 або для підприємств E5.
   > [!NOTE]
   > До Програми Microsoft 365 для бізнесу планів Microsoft 365 Бізнес Стандарт та інших планів Програми Microsoft 365 для підприємств.
- Потрібно ввімкнути [активацію на спільному комп'ютері.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

> [!NOTE]
> Крім того, можна завантажити й запустити програму [Microsoft Помічник із підтримки й відновлення,](https://aka.ms/SaRA_OfficeSCA_M365Portal) щоб інсталювати Програми Microsoft 365 для підприємств в режимі активації на спільному комп'ютері.

Докладні відомості про попередні вимоги, інструкції з настроювання та вказівки щодо настроюваних інсталяцій за допомогою засобу розгортання Office див. в статті Розгортання [Програми Microsoft 365 для підприємств](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)за допомогою служб віддалених робочих столів.

Щоб виправити помилки, пов'язані з активацією на спільному комп'ютері:

- Докладні [відомості див. в Програми Microsoft 365 для підприємств.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
- Докладні відомості див. в статті [Скидання стану активації програми Microsoft 365 для підприємств](https://go.microsoft.com/fwlink/?linkid=2109218).

Якщо потрібно інсталювати пакет Програми Microsoft 365 для підприємств RDS із ***Центр адміністрування Microsoft 365,*** у якому використовуються настройки інсталяції за замовчуванням, виконайте наведені нижче дії.

1. Перевірте, яка у вас передплата. [Дізнайтеся, як](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)це зробити.
2. За потреби перейдіть до іншої передплати. [Дізнайтеся, як](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)це зробити.
3. Якщо Office RDS-сервері вже інстальовано за допомогою будь-яких інших передплат Microsoft, видаліть його. Наприклад, відкрийте Панель **керування Видалення**  >  **програми**. Видаліть за [допомогою Помічник із підтримки й відновлення](https://aka.ms/SARA-OfficeUninstall-Alchemy) Microsoft, якщо у вас виникають проблеми.
4. На сервері RDS увійдіть у свій обліковий Центр адміністрування Microsoft 365 та інсталюйте [Програми Microsoft 365 для підприємств](https://portal.office.com/OLS/MySoftware.aspx).
5. Після Office не відкривайте  програми та не входьте в Office входу.
6. На сервері RDS увімкніть активацію на спільному комп'ютері, змінивши реєстр, виконавши такі дії:
   1. Клацніть правою кнопкою миші Windows у нижньому лівому куті екрана та виберіть команду **Виконати**. У полі Відкрити введіть **regedit** і натисніть кнопку **OK.**
   2. Коли **з'явиться** відповідний запит, натисніть кнопку Так, щоб дозволити редактор реєстру вносити зміни на пристрої.
   3. У редакторі реєстру додайте значення рядка **SharedComputerLicensing** із значенням 1 у розділі HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. На сервері RDS увійдіть як користувач і переконайтеся, що активацію на спільному комп'ютері [Програми Microsoft 365 для підприємств.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded) 
