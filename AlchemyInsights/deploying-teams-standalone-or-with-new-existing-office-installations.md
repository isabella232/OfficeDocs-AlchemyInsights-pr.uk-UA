---
title: Розгортання команд як автономних або з новими або існуючими офісними установками
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 4b843407f05db207f3b676c03c7088d3d0ba062e
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704654"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Розгортання команд як автономних або з новими або існуючими офісними установками

Microsoft teams входить до складу ***нових інсталяції*** Microsoft 365 програм для підприємств, Microsoft 365 програми для бізнесу та Office for Mac. Для отримання додаткових відомостей див. [коли Microsoft teams почне включати нові установки Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)

Крім того, починаючи з версії 1906 в щомісячному каналі, команди будуть ***додані до існуючих установок*** Microsoft 365 додатків для підприємств (і Microsoft 365 Apps для бізнесу) на пристроях під управлінням Windows, коли ви оновлюєте існуючу інсталяцію до останньої версії. Щоб дізнатися більше, перегляньте відомості [про існуючі інсталяції Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)

> [!NOTE]
> Якщо ви не хочете чекати цього розкладу розгортання, ви можете розгорнути teams як автономний для ваших користувачів, [дотримуючись цих вказівок](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) , або ви можете мати користувачів встановлювати команди для себе [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads).

Якщо ваша організація не готова розгортати команди, у нас є кроки, які можна зробити, щоб ***виключити команди*** з [нових](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) або [існуючих](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) інсталяцій Office. Якщо потрібно інсталювати групи, але не потрібно, щоб команди автоматично запускаються після інсталяції користувача, перегляньте команду [заборонити автоматичний запуск Microsoft teams після інсталяції](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Щоб ***Видалити групи*** з пристрою під керуванням Windows [, див.](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81) Щоб очистити Microsoft teams від кількох цільових машин або користувачів [, див.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)

Якщо ви користуєтеся спільними комп'ютерами, службами віддалених робочих столів (RDS) або інфраструктурою віртуального робочого стола (VDI), перегляньте [загальні комп'ютерні та VDI середовища у Microsoft teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Якщо використовується Office for Mac [, див.](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)

> [!NOTE]
> Після інсталяції команд [автоматично оновлюється](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) приблизно кожні два тижні з новими функціями та якісними оновленнями. 