---
title: Не вдається отримати доступ до спільних папок
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959515"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook не вдалося підключитися до спільних папок

Якщо доступ до спільних папок не працює для кількох користувачів, спробуйте виконати наведені нижче дії.

Підключіться до EXO PowerShell і настройте DefaultPublicFolderMailbox на обліковий запис користувача, щоб відповідати один на робочий обліковий запис користувача.

Приклад:

Отримати-поштову скриньку WorkingUser | DefaultPublicFolderMailbox FT, ефективність поштової скриньки

Проблеми з настроювання поштової скриньки-DefaultPublicFolderMailbox \<значення з попередньої команди>

Зачекайте принаймні одну годину, щоб зміни набрали сили.