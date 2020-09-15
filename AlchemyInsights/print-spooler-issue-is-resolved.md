---
title: Вирішено проблему з спулером друку
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 66b39434ef6f9ad2b8392f811704e67c1bcffd2b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801862"
---
# <a name="print-spooler-issue-is-resolved"></a>Вирішено проблему з спулером друку

Якщо ваш пристрій оновлено в ОС Windows 10  **OS Build 19041,329**, можливо, ви спостерігали проблему, коли деякі принтери не друкуватимуться. Спулеру друку може призвести до помилки або несподівано закриватися під час спроби друку, а вивід не надходить із відповідного принтера. Цю проблему вирішено в ОС збірці  **19041,331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).  

**Поточне розслідування**

Файл служби підсистеми локального центру безпеки (**Isass.exe**) може не відображатися на деяких пристроях із повідомленням про помилку "критичний системний процес, C:\WINDOWS\system32\Isass.exe, помилка з кодом стану c0000008. Тепер комп'ютер має бути перезавантажено ".  **Корпорація Майкрософт працює над дозволом і надасть оновлення в майбутньому випуску.**

Щоб отримати докладніші відомості, ознайомтеся з  [Windows 10 Version 2004 з відомими проблемами](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).