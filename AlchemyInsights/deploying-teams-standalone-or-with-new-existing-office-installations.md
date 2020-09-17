---
title: Розгортання груп як автономних або з новими або існуючими інсталяціями Office
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: c3ca4365abc41509ccf602c5b9046655706840fc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806780"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Розгортання груп як автономних або з новими або існуючими інсталяціями Office

Команди Microsoft тепер входять до складу ***нових інсталяцій*** програм Microsoft 365 для підприємств, програм Microsoft 365 для бізнесу та Office для Mac. Додаткові відомості наведено в статті [коли будуть включені команди Microsoft, які запускаються в нових інсталяціях Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Крім того, починаючи з версії 1906 у поточному каналі, команди буде ***додано до наявних інсталяцій*** програм Microsoft 365 для підприємств (а також програми Microsoft 365 для бізнесу) на пристроях під керуванням ОС Windows, коли ви оновлюєте наявну інсталяцію до найновішої версії. Докладні відомості наведено в статті [про поточні інсталяції Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Якщо ви не хочете чекати на цей графік розгортання, ви можете розгортати команди як автономні для користувачів, дотримуючись наведених [нижче інструкцій](https://docs.microsoft.com/MicrosoftTeams/msi-deployment),   або ви можете інсталювати команди для себе  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Якщо ваша організація не готова до розгортання груп, у нас є кроки, які можна виконати, щоб ***виключити команди*** з [нових](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) або [діючих](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) інсталяцій Office. Якщо потрібно інсталювати команди, але не потрібно, щоб команди запускатимуться автоматично для користувача після її інсталяції, перегляньте статтю [Заборона автоматичного запуску команди Microsoft після інсталяції](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Щоб ***Видалити команди*** з пристрою під керуванням ОС Windows, перегляньте статтю [видалення команд Microsoft](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Щоб очистити групи Microsoft із кількох цільових машин або користувачів, ознайомтеся з командою [Microsoft розгортання команд](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Якщо ви використовуєте спільні комп'ютери, служби віддалених робочих столів (RDS) або віртуальну інфраструктуру для настільних комп'ютерів (VDI), перегляньте [спільний комп'ютер і середовище VDI із командами Microsoft](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Якщо ви використовуєте Office для Mac, ознайомтеся [з командами Microsoft для інсталяції на комп'ютері Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Після інсталяції команд він [автоматично оновлюється](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) приблизно кожні два тижні з новими функціями та оновленнями якості. 