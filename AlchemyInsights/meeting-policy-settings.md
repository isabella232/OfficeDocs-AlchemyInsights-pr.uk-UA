---
title: Параметри політики наради
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704627"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Керування політиками нарад у групах Microsoft

**Примітка. у разі внесення змін до політики для користувачів може знадобитися до 24 годин.** Можливо, ви не зможете вносити зміни до щойно створених політик негайно; Зачекайте 4 години та спробуйте змінити щойно створену політику ще раз.

Політики нарад використовуються для керування функціями, доступними для учасників наради, запланованими користувачами в організації. Деякі функції політик нарад, можливо, не реалізуються в центрі адміністрування команд, але ще (ці дані позначено як "Coming Soon" у документації). У цьому випадку або якщо з'являється повідомлення про помилку "не вдалося оновити політику зараз, але повторіть спробу пізніше" в центрі адміністрування груп Microsoft, радимо використовувати PowerShell для створення або змінення політик нарад груп. 

Щоб отримати докладні відомості про політики наради, ознайомтеся з такими ресурсами:

- Щоб дізнатися про те, як створювати політики, вносити зміни та призначати користувачам політику, перегляньте статтю [керування політиками нарад в командах](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Щоб внести зміни до політики за допомогою командлетів PowerShell, перегляньте статтю [Огляд PowerShell у групах](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Потрібно використовувати [модуль "Skype для бізнесу PowerShell](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) " для нарад у групах. 
    - Перегляньте документацію за допомогою [командлетів *-cstefietingpolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) , щоб отримати докладні відомості.

