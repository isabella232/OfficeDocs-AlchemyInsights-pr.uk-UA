---
title: Пошук і видалення повідомлень електронної пошти в організації
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: bd25d9bb2af8114786503e129de105c9a0f602c98b206f01770605d1957e3a1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948904"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Пошук і видалення повідомлень електронної пошти в організації

Виконайте наведені нижче кроки.

1. Якщо ви не глобальний адміністратор, потрібно додати повідомлення, які  шукають ваш обліковий запис, до групи ролей Диспетчера витребування електронної інформації або Роль керування пошуком **відповідності.** Щоб видалити повідомлення, потрібно приєднатися  до групи ролей Керування організацією або **ролі керування пошуком і видаленням**. Дозволи на ці ролі призначаються в [Центрі безпеки & відповідності.](https://protection.office.com)
2. [Створіть пошук вмісту,](https://docs.microsoft.com/office365/securitycompliance/content-search) щоб знайти повідомлення, яке потрібно видалити.
3. [Підключення до Центру безпеки & відповідності PowerShell.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell) Якщо використовується багатофакторна автентифікація, див. Підключення в Центрі безпеки & відповідності PowerShell за допомогою [багатофакторної автентифікації.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Видаліть повідомлення: запустіть `New-ComplianceSearchAction` командлет, щоб видалити повідомлення. Видалені повідомлення переміщуються до папки "Відновлювані елементи" користувача. Приклад команди див. в розділі [Крок 3. Видалення повідомлення.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
