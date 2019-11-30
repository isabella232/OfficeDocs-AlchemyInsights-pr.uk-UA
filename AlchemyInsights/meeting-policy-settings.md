---
title: Параметри політики для нарад
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: b5599c9974eb1c112835a9f42e4ebdc926071ea2
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627595"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Керування політиками нарад у Microsoft teams

Політика для нарад використовується для керування функціями, доступними для учасників нарад, запланованих користувачами в організації. Деякі функції політики нарад можуть не реалізовуватися в центрі адміністрування команд (ці дані позначено як "скоро" у документації). У цьому випадку, або якщо ви отримуєте повідомлення про помилку "ми не можемо оновити політику прямо зараз, але повторіть спробу пізніше" у центр адміністрування Microsoft teams, рекомендовано використовувати PowerShell для створення або змінення політики для нарад, teams. 

Додаткові відомості про правила для нарад можна отримати в таких ресурсах:

- Щоб дізнатися про створення політик, внесення змін і призначення користувачів політиці [, див.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- Щоб внести зміни до політики за допомогою командлети PowerShell [, див.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - Потрібно використовувати [Skype, бізнес-PowerShell модуль](https://www.microsoft.com/download/details.aspx?id=39366) для робочих груп, наради політики. 
    - Перегляньте [документацію *-cпаросletingpolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) для отримання додаткових відомостей

**Примітка:** Зміни в політиці можуть тривати до 24 годин, щоб вони набрали сили для користувачів. Ви не зможете негайно вносити зміни до щойно створених політик; Зачекайте 4 години та спробуйте змінити знову створену політику. Якщо проблеми не виникають, спробуйте PowerShell.  