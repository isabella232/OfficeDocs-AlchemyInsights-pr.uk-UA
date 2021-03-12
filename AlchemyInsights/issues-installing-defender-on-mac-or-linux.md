---
title: Проблеми з інсталяцією Microsoft Defender на комп'ютері Mac або Linux
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
ms.openlocfilehash: a8d5ad2246b9b83e1e0a4d5be4dd8bb41c16e734
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "50714320"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Проблеми з інсталяцією Microsoft Defender на комп'ютері Mac або Linux

**Mac**

- Переконайтеся, що Системні вимоги виконуються, перш ніж інсталювати програму Microsoft Defender АТФ для Mac. Щоб отримати докладні відомості, Дізнайтеся, [як інсталювати програму Microsoft DEFENDER АТФ для Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).  
- Перегляньте інформацію у файлі: "/Library/Logs/Microsoft/mdatp/install.log".

**Linux**

- Переконайтеся, що Системні вимоги виконуються, перш ніж інсталювати програму Microsoft Defender АТФ для Linux. Щоб отримати докладні відомості, Дізнайтеся, [як інсталювати програму Microsoft DEFENDER АТФ для Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements). 
- Щоб перевірити, чи запущено службу MDATP, перегляньте статтю [Помилка інсталяції](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).  
    Щоб усунути неполадки та вирішити проблеми, якщо служба не запущена, перегляньте [кроки з усунення несправностей, якщо служба mdatp не запущена](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).
- Щоб перевірити конфігурацію клієнта, у якому перевіряється стан справності продукту, а також для запуску тесту виявлення в текстовому файлі EICAR, перегляньте статтю [Конфігурація клієнта](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).  

    **Примітка** . Щоб переглянути список підтримуваних файлових систем для роботи з доступом, ознайомтеся з [програмою Microsoft DEFENDER АТФ для Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).