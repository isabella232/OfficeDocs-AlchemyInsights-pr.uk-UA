---
title: Проблеми з видаленням з'єднуваного або дезахизаційного пристрою з інвентарного списку пристроїв
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 13865acb75b60a824c1dde9427c11471e980ea9e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324465"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a>Проблеми з видаленням з'єднуваного або дезахизаційного пристрою з інвентарного списку пристроїв

Захисник Microsoft для кінцевої точки наразі не дає змоги вручну видалити запис пристрою з адаптивного або декомпіляційного пристрою з інвентарного списку пристроїв.

З міркуваннями безпеки пристрій залишається на порталі як історичний запис протягом 180 днів. Проте дані пристрою одужуються відповідно до налаштованого періоду збереження.

**Примітка.** Після семи днів адаптивний пристрій автоматично переключиться на **неактивний** стан. Крім того, пристрої, неактивні за останні 30 днів, не впливають на дані, які відображають загрозу вашої організації та оцінку ризику керування вразливістю або Microsoft Secure Score для пристроїв.
 
Якщо ви все одно не хочете бачити певні пристрої в поданні інвентарного списку пристроїв, спробуйте розмістити тег пристрою, щоб відфільтрувати знятий пристрій із подання "Запаси пристроїв".

Докладні відомості:

[З'єднувачі зі служби кінцевих точок Microsoft Defender](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/offboard-machines.md)

[Вплив оцінок у загрозі та вразливості](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[Виправлення незмінних датчиків у Microsoft Defender для кінцевої точки](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[Ефективне використання тегів (частина 1)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[Ефективне використання тегів (частина 2)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[Ефективне використання тегів (частина 3)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




