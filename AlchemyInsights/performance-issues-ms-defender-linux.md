---
title: Проблеми з продуктивністю кінцевої точки для Захисника Microsoft у Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794222"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a>Проблеми з продуктивністю кінцевої точки для Захисника Microsoft у Linux

У цій статті описано кроки з визначення проблем із продуктивністю для кінцевої точки Microsoft Defender у Linux.

Спочатку переконайтеся, що проблему, з якою виникла проблема, вирішено в найновішій [версії](/microsoft-365/security/defender-endpoint/linux-whatsnew). 

Відомості про початок дослідження див. в статті Усунення несправностей із продуктивністю [microsoft Defender для кінцевої точки в Linux.](/microsoft-365/security/defender-endpoint/linux-support-perf)

## <a name="exclusions"></a>Винятки

Винятки можуть допомогти знизити продуктивність. Перш ніж почати, перегляньте винятки, щоб отримати додаткову інформацію про ризик і документацію.

Докладні відомості див. в статті Налаштування та перевірка винятків для Microsoft [Defender для кінцевої точки в Linux.](/microsoft-365/security/defender-endpoint/linux-exclusions)

Якщо у вас є кілька файлів & папок, які потрібно виключити, і всі вони на одній горині, може бути легше виключити байт. Починаючи з лютого випуску 101.22.80, ви можете виключити всю точку встановлення.

Наприклад, якщо /mnt/backup – це байтна точка, до списку виключених елементів можна додати /mnt/backup, запустивши таку команду:

`$ mdatp exclusion folder add –path /mnt/backup`

**Примітка.** Додавання винятків підвищує ризик того, що зловмисне програмне забезпечення не виявляється, і його потрібно обробляти та впроваджувати з обережністю.

## <a name="need-help"></a>Потрібна допомога?

Щоб допомогти вам у найефективнішому способі, зберіть діагностичні дані, перш ніж відкривати інцидент служби підтримки.
