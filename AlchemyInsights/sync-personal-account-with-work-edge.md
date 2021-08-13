---
title: Надання користувачу змоги синхронізувати особистий обліковий запис із робочим обліковим записом у Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9127"
- "9004429"
ms.openlocfilehash: da435b37b689e97ca51ce5cf94eb7e7d71eb972060526989239310fac1460628
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813410"
---
# <a name="enable-a-user-to-sync-a-personal-account-with-the-work-account-in-microsoft-edge"></a>Надання користувачу змоги синхронізувати особистий обліковий запис із робочим обліковим записом у Microsoft Edge

Переконайтеся, що ви відповідаєте таким умовам:

- Функцію корпоративного роумінга штату ввімкнуто в Центрі адміністрування Azure Active Directory, яка вимагає передплати на Azure Active Directory Premium або Enterprise Mobility + Security (EMS). Докладні відомості див. в [цій](/azure/active-directory/devices/enterprise-state-roaming-enable)Azure Active Directory.
- Виконано одну або обидві з наведених нижче умов.
    - Службу Azure Information Protection увімкнуто для вашого клієнта. Докладні відомості [див. в Azure Rights Management на сторінці Активація захисту Центр адміністрування Microsoft 365.](/azure/information-protection/activate-office365)
    - Функцію Azure Active Directory enterprise State Roaming (ESR) увімкнуто для будь-якого користувача або клієнта. Докладні відомості див. в [розділах Що таке роумінг корпоративного стану?](/azure/active-directory/devices/enterprise-state-roaming-overview).

Якщо І AIP, і ESR вимкнуто, з'являється повідомлення про те, що користувачі, які синхронізуються, недоступні для своїх облікових записів.
