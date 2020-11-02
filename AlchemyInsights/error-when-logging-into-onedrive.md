---
title: Помилка 0x8004de40 під час запуску OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823122"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>Помилка 0x8004de40 під час запуску OneDrive

Якщо під час входу в службу OneDrive з'являється повідомлення про помилку **0x8004de40** , перезавантажте комп'ютер під час підключення до робочого або навчального домену. Якщо ви отримали цю помилку після перезавантаження, випробуйте цей час, коли підключаєтеся до робочого або навчального домену, виконайте такі дії:

1. Натисніть кнопку Пуск і введіть **CMD** або **командний рядок**  у полі пошуку, клацніть правою кнопкою миші у програмі командний рядок і виберіть команду  **Запуск із правами адміністратора** . Якщо з'явиться запит на введення пароля адміністратора або підтвердження, введіть пароль або натисніть кнопку **дозволити** .  

2. У вікні командного рядка введіть **dsregcmd/Leave**  і зачекайте, доки команда завершиться. Потім введіть **dsregcmd/JOIN** і зачекайте, доки команда завершиться.
3. Перезавантажте комп'ютер.
