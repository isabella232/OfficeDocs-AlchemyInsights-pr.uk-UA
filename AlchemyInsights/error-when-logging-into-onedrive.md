---
title: 0x8004de40 під час запуску OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: 23c57356c8bd94c1cbafb538c9318208429754115a7c4e88abc93d293b5ea6e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946600"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 під час запуску OneDrive

Якщо під час входу в **0x8004de40 OneDrive** з'являється повідомлення про помилку, перезавантажте комп'ютер, підключивши його до робочого або навчального домену. Якщо після перезавантаження з'являється таке повідомлення про помилку, спробуйте таке під час підключення до робочого або навчального домену:

1. Натисніть кнопку Пуск і введіть **cmd** або **командний** рядок у полі пошуку, клацніть правою кнопкою миші програму командного рядка та виберіть **команду Запустити з правами адміністратора.** Якщо буде запропоновано ввести пароль адміністратора або підтвердження, введіть пароль або натисніть кнопку **Дозволити.**  

2. У вікні Командний рядок введіть **dsregcmd /leave**  і зачекайте, доки не завершиться команда. Потім введіть **dsregcmd /join і** дочекайтеся завершення команди.
3. Перезавантажте комп'ютер.
