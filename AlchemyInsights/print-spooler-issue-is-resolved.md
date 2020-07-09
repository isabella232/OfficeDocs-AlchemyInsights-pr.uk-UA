---
title: Усунуто проблему спулера друку
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 53b1c9a8efa3cc978af8b602c8ed90430042186a
ms.sourcegitcommit: 4265a9e79db6c2a396aa80ec0ebd467bbaadf366
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/08/2020
ms.locfileid: "45088529"
---
# <a name="print-spooler-issue-is-resolved"></a>Усунуто проблему спулера друку

Якщо пристрій було оновлено з ОС Windows 10 **OS Build 19041,329**, можливо, спостерігається проблема, коли деякі принтери не друкувати. Спулеру друку може викинути помилку або несподівано закрити під час спроби друку, і вихід із відповідного принтера не надходить. Цю проблему усунуто в ОС збірка **19041,331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).  

**Поточне розслідування**

На деяких пристроях, з повідомленням про помилку, може не вдатися до**Isass.exe**LSASS, а не вдалося виконати на деякі пристрої, "критичний системний процес, C:\WINDOWS\system32\Isass.exe, помилка з кодом стану c0000008". Машина тепер має бути перезапущено ".  **Корпорація Майкрософт працює над роздільною здатністю та надасть оновлення в майбутньому випуску.**

Щоб отримати додаткові відомості, будь ласка, ознайомтеся з [Windows 10 версії 2004 відомі проблеми](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).