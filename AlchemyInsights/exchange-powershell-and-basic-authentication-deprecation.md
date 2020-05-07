---
title: Exchange PowerShell і припинення підтримки базової автентифікації
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015710"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell і припинення підтримки базової автентифікації

Найновіші відомості про підключення до Exchange Online PowerShell без використання базової автентифікації [див. тут](https://aka.ms/psbasicauth).

Зверніть увагу, що базову автентифікацію все одно потрібно ввімкнути на клієнтському комп'ютері.
У новому модулі PowerShell V2 використовується сучасна автентифікація, щоб установити підключення для ввімкнення всіх командлетів V2 на основі REST. Крім того, можна отримати доступ до старіших командлетів PowerShell (RPS), створивши віддалений сеанс PowerShell. Щоб створити сеанс RPS на комп'ютері з ОС Windows, необхідно ввімкнути базову автентифікацію WinRM на клієнтському комп’ютері, хоча в модулі використовується механізм сучасної автентифікації для автентифікації в службі. Канал базової автентифікації WinRM використовується для транспортування маркерів сучасної автентифікації. Якщо базову автентифікацію WinRM вимкнуто на клієнтському комп'ютері, нові командлети V2 продовжуватимуть працювати (на відміну від старіших командлетів RPS).
