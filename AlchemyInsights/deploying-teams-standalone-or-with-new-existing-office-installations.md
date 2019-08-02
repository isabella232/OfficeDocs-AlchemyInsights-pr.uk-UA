---
title: Розгортання команди, як автономний або з нової або наявної інсталяції Office
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 08/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 3318e1b17cc99e927e1011f7ca9eca8dec616d59
ms.sourcegitcommit: 4600dd4fb577bf5f5482a24616c2d9a6b81e8052
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/01/2019
ms.locfileid: "36054251"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Розгортання команди, як автономний або з нової або наявної інсталяції Office

Microsoft команди в даний час включено в рамках ***нової установки*** Office 365 ProPlus Office 365 бізнес та Office для Mac. Докладніше, перегляньте [коли команди Microsoft почнуть включаються нові установки Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)

Крім того, починаючи з версії 1906 щомісяця каналу, команди буде ***додано до існуючих установок*** Office 365 ProPlus (та Office 365 бізнесу) на пристроях під управлінням Windows, коли ви оновлюєте наявну інсталяцію останньої версії. Докладніше, перегляньте [як щодо існуючих установок Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)

> [!NOTE]
> Якщо ви не хочете чекати, поки цей розклад свиті, щоб розгорнути команди як автономний для ваших користувачів, [виконайте наступні інструкції](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) або ви можете мати ваші користувачі встановити команд для себе від [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads).

Якщо ваша організація не готові, щоб розгорнути команди, ми маємо на кроків можна виключити ***команд*** з [нової](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) або [наявної](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) інсталяції Office. Якщо ви хочете, щоб команди, щоб бути встановлені, але не хочете команд для автоматичного запуску для користувача, після інсталяції, побачити [Запобігти Microsoft збірними починаючи автоматично після встановлення](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

***Видалення групи*** з пристрою під керуванням Windows переглянути [Видалити Microsoft команд](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Для очищення команди Microsoft з кількох цільових комп'ютерах або користувачів побачити [очищення команди Microsoft розгортання](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Якщо ви використовуєте спільних комп'ютерах, віддалений робочий стіл служб (РДС) або віртуальний робочий стіл інфраструктури (VDI), зверніться до [спільний комп'ютер і VDI середовищах з Microsoft команд](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Якщо ви використовуєте Office for Mac, див [Microsoft команд установок на Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Після цього команди це [автоматично оновлюється](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) приблизно кожні два тижні з новими можливостями і якість оновлень. 