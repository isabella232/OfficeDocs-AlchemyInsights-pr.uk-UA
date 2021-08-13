---
title: Teams не запускати
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/4/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12673"
- "9007646"
ms.openlocfilehash: a37f980e700090da8199c703216af6f04f4aca464c21870beb3e907dd7b2d491
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813362"
---
# <a name="teams-doesnt-launch"></a>Teams не запускати

Якщо спробувати відкрити файл, Microsoft Teams запускати його ніколи не відкривається, спробуйте зробити ось що:

1. Перейдіть до **%appdata%\Microsoft\Teams.**
1. Видаліть вміст папки.
1. Перезавантажте комп'ютер і спробуйте запустити Teams.

Можливо, знадобиться повторно інсталювати Teams. Щоб повторно інсталювати пакет:

1. Видаліть Teams за допомогою Панелі керування.
1. Перейдіть до **%appdata%\Microsoft\Teams\Кеш програм.**
1. Видаліть вміст папки.
1. Перейдіть до **%appdata%\Microsoft\teams\Cache.**
1. Видаліть вміст папки.
1. Перезавантажте комп'ютер, а потім завантажте та інсталюйте Teams.

Якщо потрібно виконати діагностичну діагностику для певного користувача, який не може ввійти, почніть пошук за ключовим словом **TeamsUserUnableToSignIn** і дотримуйтеся вказівок.