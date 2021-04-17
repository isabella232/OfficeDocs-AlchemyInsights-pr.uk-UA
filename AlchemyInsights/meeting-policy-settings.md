---
title: Параметри політики нарад
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825464"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Керування політиками нарад у Microsoft Teams

**Примітка. Зміни політики набирають сили для користувачів протягом 24 годин.** Можливо, ви не зможете вносити зміни відразу до ново створених політик. зачекайте 4 години та спробуйте знову змінити щойно створену політику.

Політики нарад використовуються, щоб контролювати функції, доступні учасникам наради для нарад, які запланували користувачі у вашій організації. Деякі функції політик нарад можуть ще не впроваджуватись у Центрі адміністрування Teams (вони позначені як "незабаром" у документації). У цьому випадку або якщо з'являється таке повідомлення про помилку, як "Не вдалося оновити політику зараз, але повторити спробу пізніше" в Центрі адміністрування Microsoft Teams, радимо створити або змінити політики нарад Teams за допомогою PowerShell. 

Докладні відомості про політики нарад див. в таких ресурсах:

- Докладні відомості про створення політик, внесення змін і призначення користувачів політиці див. в розділі Керування [політиками нарад у Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- Відомості про змінення політики за допомогою командлетів PowerShell див. в [цьому огляді.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - Потрібно використовувати модуль [PowerShell "Skype для бізнесу" для](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) політик нарад Teams. 
    - Докладні відомості див. в документації про командлети [*-CsTeamsMeetingPolicy.](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)

