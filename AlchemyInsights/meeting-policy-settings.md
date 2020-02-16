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
- "9000734"
- "2657"
ms.openlocfilehash: 509bd0c686830c04ed27f97372411677c0a7f4a4
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/15/2020
ms.locfileid: "42042865"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Керування політиками нарад у Microsoft teams

**Примітка: це може зайняти до 24 годин, щоб зміни політики набрали сили для користувачів.** Ви не зможете негайно вносити зміни до щойно створених політик; Зачекайте 4 години та спробуйте змінити знову створену політику.

Політика для нарад використовується для керування функціями, доступними для учасників нарад, запланованих користувачами в організації. Деякі функції політики нарад можуть не реалізовуватися в центрі адміністрування команд (ці дані позначено як "скоро" у документації). У цьому випадку, або якщо ви отримуєте повідомлення про помилку "ми не можемо оновити політику прямо зараз, але повторіть спробу пізніше" у центр адміністрування Microsoft teams, рекомендовано використовувати PowerShell для створення або змінення політики для нарад, teams. 

Додаткові відомості про правила для нарад можна отримати в таких ресурсах:

- Щоб дізнатися про створення політик, внесення змін і призначення користувачів політиці [, див.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- Щоб внести зміни до політики за допомогою командлети PowerShell [, див.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - Потрібно використовувати [Skype, бізнес-PowerShell модуль](https://www.microsoft.com/download/details.aspx?id=39366) для робочих груп, наради політики. 
    - Перегляньте [документацію *-cпаросletingpolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) для отримання додаткових відомостей

