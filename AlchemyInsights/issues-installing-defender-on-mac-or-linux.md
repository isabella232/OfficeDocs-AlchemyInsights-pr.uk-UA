---
title: Проблеми з інсталяцією Захисника Microsoft на комп'ютері Mac або Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: ae17caa4be7809b591be9f9c042186f67828aa3c36a3d17332806e4d92545dc6
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/11/2021
ms.locfileid: "57898629"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Проблеми з інсталяцією Захисника Microsoft на комп'ютері Mac або Linux

**Mac**

- Перш ніж інсталювати РЗЗ Microsoft Defender для Mac, переконайтеся, що вимоги до системи виконано. Докладні відомості див. в статті Інсталяція РЗЗ Microsoft [Defender для Mac.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)  
- Перегляньте відомості у файлі: "/Library/Logs/Microsoft/mdatp/install.log".

**Linux**

- Перш ніж інсталювати РВП для Linux для Захисника Microsoft Defender, переконайтеся, що вимоги до системи виконано. Докладні відомості див. [в статті Інсталяція MDATP для Linux.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements) 
- Відомості про те, як перевірити, чи запущено службу MDATP, див. в [цьому статі.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)  
    Щоб усунути несправностей, пов'язаних із несправністю, якщо не запущено службу mdatp, див. статтею Кроки з усунення несправностей, якщо службу [mdatp не запущено.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)
- Щоб дізнатися, як перевірити конфігурацію клієнта, яка перевіряє справність продукту, і пройти [](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration)перевірку виявлення в текстовому файлі EICAR, див. рис.  

    **Примітка** Список підтримуваних файлових систем для дій із доступом див. в статті [РВП Microsoft Defender для Linux.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)