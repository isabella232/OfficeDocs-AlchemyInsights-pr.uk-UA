---
title: Віддалене вирішення проблем із пристроями переходу для Windows 10 для захисту від досвідчених загроз Microsoft Defender
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694841"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a>Віддалене вирішення проблем із пристроями переходу для Windows 10 для захисту від досвідчених загроз Microsoft Defender

Якщо ви можете отримати доступ до віддаленого комп'ютера, виконайте наведені нижче дії.

1. Завантажте засіб діагностики засобу [аналізу підключення клієнта](https://go.microsoft.com/fwlink/?linkid=2143466) .
2. Розпакуйте та запустіть програму MDATPAnalyzer. cmd.
3. Знайдіть журнал діагностики в папці Mdatpdreclireрезультуючий, що є тією самою папкою, де завантажувалася засіб аналізу.
4. Щоб отримати проблеми з настройками підключення або проксі-сервера Інтернету, ознайомтеся з файлом журналу MDATPClientAnalyzer.txt.

Щоб дізнатися більше, ознайомтеся [з проблемами з переходу машини](https://go.microsoft.com/fwlink/?linkid=2143634).
