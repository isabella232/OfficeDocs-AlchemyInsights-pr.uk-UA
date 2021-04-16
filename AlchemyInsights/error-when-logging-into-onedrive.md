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
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813673"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 під час запуску OneDrive

Якщо під час входу **у OneDrive 0x8004de40** з'являється повідомлення про помилку, перезавантажте комп'ютер під час підключення до робочого або навчального домену. Якщо після перезавантаження з'являється таке повідомлення про помилку, спробуйте таке під час підключення до робочого або навчального домену:

1. Натисніть кнопку Пуск і введіть **cmd** або **командний** рядок у полі пошуку, клацніть правою кнопкою миші програму командного рядка та виберіть **команду Запустити з правами адміністратора.** Якщо буде запропоновано ввести пароль адміністратора або підтвердження, введіть пароль або натисніть кнопку **Дозволити.**  

2. У вікні Командний рядок введіть **dsregcmd /leave**  і зачекайте, доки не завершиться команда. Потім введіть **dsregcmd /join і** дочекайтеся завершення команди.
3. Перезавантажте комп'ютер.
