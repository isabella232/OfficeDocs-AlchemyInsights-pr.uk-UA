---
title: Увімкнення Teams вебінарів
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/04/2021
ms.locfileid: "52794035"
---
# <a name="enable-teams-webinars"></a>Увімкнення Teams вебінарів

Вебінари ввімкнуто за замовчуванням. За допомогою команд PowerShell можна впорядковувати та Teams Teams для вебінарів.

- Усі користувачі, які можуть створити нараду, також можуть створювати веб-наради. Щоб керувати списком користувачів, які можуть планувати Teams, використовуйте *параметр AllowMeetingRegistration.* 
- За замовчуванням *параметр WhoCanRegister* увімкнуто та встановлено значення **Усі.** Щоб вимкнути реєстрацію наради, установіть для параметра *AllowMeetingRegistration значення* **False (Хибість).**

Щоб змінити ці параметри, потрібно інсталювати Teams [PowerShell.](/microsoftteams/teams-powershell-install) Крім того, політики нарад застосовуються Teams вебінарів. Наприклад, якщо анонімне приєднання вимкнуто в параметрах наради, анонімні користувачі не можуть приєднатися до вебінарів.

Докладні відомості про настроювання користувачів, які можуть зареєструватися для вебінарів, див. в статтях Настроювання користувачів, які [можуть зареєструватися для вебінарів.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars) Докладні відомості про параметри для microsoft Lists див. в [статті Параметри керування для Microsoft Lists.](/sharepoint/control-lists)