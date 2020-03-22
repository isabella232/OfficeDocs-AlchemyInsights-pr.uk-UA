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
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891770"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook не вдалося підключитися до спільних папок

Якщо доступ до спільних папок не працює для деяких користувачів, спробуйте виконати наведені нижче дії.

Підключіться до EXO PowerShell і настройте параметр DefaultPublicFolderMailbox на обліковий запис користувача, щоб зіставити параметр у робочий обліковий запис користувача.

Приклад:

Отримати-поштову скриньку WorkingUser | DefaultPublicFolderMailbox FT, ефективність поштової скриньки

Проблеми з настроювання поштової скриньки-DefaultPublicFolderMailbox \<значення з попередньої команди>

Зачекайте принаймні одну годину, щоб зміни набрали сили.

Якщо проблема залишається, будь ласка, дотримуйтесь [цієї процедури](https://aka.ms/pfcte) для усунення проблем із доступом до спільних папок, використовуючи Outlook.