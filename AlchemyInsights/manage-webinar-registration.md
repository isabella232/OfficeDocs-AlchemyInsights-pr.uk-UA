---
title: Керування реєстрацією веб-inарів
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794142"
---
# <a name="manage-webinar-registration"></a>Керування реєстрацією веб-inарів

Ви можете керувати списком користувачів, які Teams вебінарів, використовуючи Teams команд PowerShell. Відомості про те Teams, як інсталювати PowerShell, [Teams PowerShell.](/microsoftteams/teams-powershell-install) 

За замовчуванням *параметр WhoCanRegister* увімкнуто та встановлено значення **EveryoneInCompany.** Щоб дозволити реєструвати всіх користувачів, зокрема анонімних користувачів, потрібно вибрати для параметра Політика наради значення **Усі** за допомогою команди PowerShell:

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**Примітка.** Якщо анонімне приєднання вимкнуто в параметрах наради, анонімні користувачі не можуть приєднатися до вебінарів. Докладні відомості та ввімкнення цієї настройки див. в розділі [Керування параметрами наради Microsoft Teams](/microsoftteams/meeting-settings-in-teams).

Щоб вимкнути реєстрацію наради, установіть для параметра *AllowMeetingRegistration значення* **False (Хибість).**

Докладні відомості про настроювання користувачів, які можуть зареєструватися для вебінарів, див. в статтях Настроювання користувачів, які [можуть зареєструватися для вебінарів.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars) Докладні відомості про параметри для microsoft Lists див. в [статті Параметри керування для Microsoft Lists.](/sharepoint/control-lists)
