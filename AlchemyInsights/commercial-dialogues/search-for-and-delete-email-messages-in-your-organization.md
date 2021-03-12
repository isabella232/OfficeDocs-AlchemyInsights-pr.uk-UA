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
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750021"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Пошук і видалення повідомлень електронної пошти в організації

Виконайте наведені нижче кроки.

1. Якщо ви не є глобальним адміністратором, щоб знайти повідомлення, які потрібно додати до вашого облікового запису, до рольової **групи «Диспетчер** Витребування» або **ролі керування відповідністю**. Щоб видалити повідомлення, потрібно приєднатися до рольової групи " **Керування організацією** " або " **Пошук і очищення**". Дозволи для цих ролей призначено в [центрі відповідності & безпеки.](https://protection.office.com)
2. [Створіть пошук вмісту](https://docs.microsoft.com/office365/securitycompliance/content-search) , щоб знайти повідомлення, яке потрібно видалити.
3. [Підключення до центру безпеки та відповідності & PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell). Якщо ви використовуєте МЗС, ознайомтеся з наведеними нижче вказівками: [підключення до центру безпеки & відповідність PowerShell за допомогою багатофакторної автентифікації](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Видаліть повідомлення: запустіть `New-ComplianceSearchAction` командлет, щоб видалити повідомлення. Видалені повідомлення переміщуються до папки «Відновлювані елементи» користувача. У полі приклад виберіть команду [крок 3: видалення повідомлення.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
