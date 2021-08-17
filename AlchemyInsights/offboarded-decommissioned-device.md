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
ms.openlocfilehash: 6eb59d16a1dab2de0e7a44faf9b34be6432342f9e20c94b6932e69e937751add
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/11/2021
ms.locfileid: "57892024"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a>Проблеми з видаленням з'єднуваного або дезахизаційного пристрою з інвентарного списку пристроїв

Захисник Microsoft для кінцевої точки наразі не дозволяє вручну видалити запис пристрою з адаптивного або декомпіляційного пристрою з інвентарного списку пристроїв.

З міркуваннями безпеки пристрій залишається на порталі як історичний запис протягом 180 днів. Проте дані пристрою одужуються відповідно до налаштованого періоду збереження.

**Примітка.** Після семи днів адаптивний пристрій автоматично переключиться на **неактивний** стан. Крім того, дані, які відображають результати виставлення рахунку або Microsoft Secure Score для пристроїв, не активуються за керування загрозами та вразливостями останні 30 днів.
 
Якщо ви все одно не хочете бачити певні пристрої в поданні інвентарного списку пристроїв, спробуйте розмістити тег пристрою, щоб відфільтрувати знятий пристрій із подання "Запаси пристроїв".

Докладні відомості:

[З'єднувачі зі служби кінцевих точок Microsoft Defender](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/offboard-machines.md)

[Оцінка експозиції в керування загрозами та вразливостями](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[Виправлення незмінних датчиків у Microsoft Defender для кінцевої точки](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[Ефективне використання тегів (частина 1)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[Ефективне використання тегів (частина 2)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[Ефективне використання тегів (частина 3)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




