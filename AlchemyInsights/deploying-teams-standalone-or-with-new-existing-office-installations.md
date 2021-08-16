---
title: Розгортання Teams окремо або з новими або наявними пакетами Office інсталяції
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
ms.openlocfilehash: e8baefafc1c2f9583345779c5ae7a9d3d0e05c4b3b7e1b3a74a9a22f7ceed02a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102223"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Розгортання Teams окремо або з новими або наявними пакетами Office інсталяції

Microsoft Teams тепер включено до складу нових інсталяцій пакетів Програми Microsoft 365 для підприємств, Програми Microsoft 365 для бізнесу і Office для Mac.  Докладні відомості див. в Microsoft Teams включення до [нових інсталяцій Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Крім того, починаючи з версії 1906 року на поточний  канал, Teams буде додано до наявних інсталяцій Програми Microsoft 365 для підприємств (і Програми Microsoft 365 для бізнесу) на пристроях із Windows після оновлення наявної інсталяції до найновішої версії. Докладні відомості [див. в Office.](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Якщо ви не бажаєте чекати на цей графік розгортання, можна розгорнути програму [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) Teams як окремо для користувачів, виконавши ці вказівки або запропонуйте користувачам інсталювати пакет Teams самостійно [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) з .

Якщо ваша організація ще не готова розгорнути Teams, ми вживаємо заходів, [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) щоб [](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) виключити Teams з нових або наявних інсталяцій Office.  Якщо потрібно Teams, але не бажаєте, щоб програма Teams автоматично запускала для користувача після інсталяції, див. 30. заборона автоматичного Microsoft Teams після [інсталяції.](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)

Відомості ***про Teams*** видалення з пристрою під керуванням Windows див. в розділі Видалення [Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Щоб видалити Microsoft Teams кількома цільовими комп'ютерами або користувачами, див. [Microsoft Teams очищення розгортання.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)

Якщо використовується спільні комп'ютери, служби віддалених робочих столів (RDS) або інфраструктура віртуальних робочих столів (VDI), див. розділ Спільні комп'ютери та середовища VDI із [Microsoft Teams.](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)

Якщо ви використовуєте пакет Office для Mac, див. Microsoft Teams [на комп'ютері Mac.](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)

> [!NOTE]
> Після Teams оновлення автоматично оновлюється [](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) приблизно кожні два тижні завдяки новим функціям і оновленням якості. 