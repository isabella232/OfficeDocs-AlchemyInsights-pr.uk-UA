---
title: Усунуто проблему спулера друку
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
ms.openlocfilehash: 73ff86928c043dd41f49d456d30c2fcf7947bd4cb304d0456c634d4fa5808239
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911359"
---
# <a name="print-spooler-issue-is-resolved"></a>Усунуто проблему спулера друку

Якщо на пристрої оновлено збірку Windows 10 **ОС 19041.329,** можливо, ви помітили проблему, через яку не вдається надрукувати певні принтери.   Спулер друку може кинути помилку або несподівано закритися під час спроби друку, а вихідні дані не надходять із відповідного принтера. Цю проблему вирішено в збірках ОС **19041.331**, [KB4567523.](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523)  

**Триває дослідження**

Файл служби підсистеми Локальної системи безпеки (LSASS)**(Isass.exe)** може не вдатися на деяких пристроях із повідомленням про помилку "Критичний системний процес, C:\WINDOWS\system32\Isass.exe, помилка з кодом стану c0000008". Тепер потрібно перезавантажити комп'ютер".  **Корпорація Майкрософт працює над вирішенням проблеми та надаватиме оновлення в майбутніх випусках.**

Докладні відомості див. в Windows 10 [версії 2004.](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc)