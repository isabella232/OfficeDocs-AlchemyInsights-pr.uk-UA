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
ms.openlocfilehash: 9d928a3bf58dedc3aaf231c8a051f87b0bbdf438
ms.sourcegitcommit: 391052026a6ce7646926d233d0fd9ba135088f79
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/01/2021
ms.locfileid: "60041027"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Розгортання Програми Microsoft 365 для підприємств для спільного використання в службах RDS, Термінал Server або VDI

Щоб розгорнути Програми Microsoft 365 служби віддалених робочих столів (RDS), раніше використовується служба терміналів, потрібно:

- Скористайтеся простим виправленням, щоб увімкнути TLS 1.2 за замовчуванням, якщо використовується попередня версія Windows (наприклад, Windows 7 із пакетом оновлень 1 (SP1), Windows Server 2008 R2). Докладні відомості про просте виправлення та докладні відомості див. в статтях Оновлення для ввімкнення [протоколів TLS 1.1 і TLS 1.2](https://support.microsoft.com/en-us/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392#bkmk_easy)як безпечних протоколів за замовчуванням у WindowsHTTP у Windows. 
- Маєте план, який включає Програми Microsoft 365 для підприємств (раніше – Office 365 Plus). Наприклад, плани Office 365 E3 чи Microsoft 365 E5, які включають класичну версію Project чи Visio, наприклад Project (план 3) чи Visio (план 2) чи план Microsoft 365 Business преміум, який також включає Програми Microsoft 365 для бізнесу.
- Увімкнути активацію на спільному комп'ютері. Докладні відомості див. в [огляді активації на спільному комп'Програми Microsoft 365.](https://docs.microsoft.com/deployoffice/overview-shared-computer-activation)

**Примітка.** Щоб інсталювати Програми Microsoft 365 в режимі активації на спільному комп'ютері, завантажте та запустіть [програму Microsoft Помічник із підтримки й відновлення](https://docs.microsoft.com/alchemyinsights/deploy-o365-remotely-to-rds). Докладні відомості про попередні вимоги, інструкції з настроювання та вказівки з настроювання інсталяцій за допомогою засобу розгортання Office див. в статті Розгортання [Програми Microsoft 365](https://docs.microsoft.com/deployoffice/deploy-microsoft-365-apps-remote-desktop-services)за допомогою служб віддалених робочих столів.

Відомості про виправлення помилок, пов'язаних з активацією на спільному комп'ютері, див. в статтях:

- [Виправлення неполадок з активацією на спільному комп'ютері Програми Microsoft 365](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation)
- [Скидання Програми Microsoft 365 для підприємств стану активації](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state)

Якщо потрібно інсталювати пакет Програми Microsoft 365 RDS із Центр адміністрування Microsoft 365, у якому використовуються стандартні параметри інсталяції, виконайте такі дії:

1. Перевірте, Microsoft 365 план. Докладні відомості див. [в відомості про те, як дізнатися, яка в мене передплата?](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).

1. За потреби змініть план Microsoft 365. Докладні відомості див. [в статтях Оновлення до іншого плану.](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan)

1. Якщо Програми Microsoft 365 RDS-сервер уже інстальовано за допомогою будь-яких інших несумісних планів, видаліть його, перейшовте на Панель   >  **керування Видалення програми**. Якщо у вас виникають проблеми, видаліть їх, завантаживши [microsoft Помічник із підтримки й відновлення](https://aka.ms/SARA-OfficeUninstall-Alchemy).

1. На сервері RDS увійдіть у свій обліковий Центр адміністрування Microsoft 365 та інсталюйте [Office](https://portal.office.com/OLS/MySoftware.aspx).

   Після Office не відкривайте програми та не входьте в Office програми.

1. На сервері RDS увімкніть активацію на спільному комп'ютері, змінивши реєстр:

   1. Клацніть правою кнопкою миші Windows у нижньому лівому куті екрана та виберіть команду **Виконати**. У полі Відкрити введіть **regedit** і натисніть кнопку **OK.**

   1. Коли з'явиться запит на дозвіл редактора реєстру вносити зміни на пристрої, натисніть **кнопку Так**.

   1. У редакторі реєстру в розділі HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration додайте значення рядка **SharedComputerLicensing** із значенням **1.**

1. На сервері RDS увійдіть як користувач і переконайтеся, що активацію на спільному комп'ютері Програми Microsoft 365. 

   Докладні відомості див. в [відомості про те, як перевірити, чи активовано](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation#verify-that-shared-computer-activation-is-enabled-for-microsoft-365-apps)активацію на спільному комп'ютері Програми Microsoft 365.