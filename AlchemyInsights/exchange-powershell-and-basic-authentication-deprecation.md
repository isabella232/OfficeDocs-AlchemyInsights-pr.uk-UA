---
title: Exchange PowerShell і припинення підтримки базової автентифікації
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813493"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell і припинення підтримки базової автентифікації

Найновіші відомості про підключення до Exchange Online PowerShell без використання базової автентифікації [див. тут](https://aka.ms/exops-docs). Модуль PowerShell V2 не використовує базову автентифікацію.

Зверніть увагу, що базову автентифікацію все одно потрібно ввімкнути на клієнтському комп'ютері.
У новому модулі PowerShell V2 використовується сучасна автентифікація, щоб установити підключення для ввімкнення всіх командлетів V2 на основі REST. Крім того, можна отримати доступ до старіших командлетів PowerShell (RPS), створивши віддалений сеанс PowerShell. Щоб створити сеанс RPS на комп'ютері з ОС Windows, необхідно ввімкнути базову автентифікацію WinRM на клієнтському комп’ютері, хоча в модулі використовується механізм сучасної автентифікації для автентифікації в службі. Канал базової автентифікації WinRM використовується для транспортування маркерів сучасної автентифікації. Якщо базову автентифікацію WinRM вимкнуто на клієнтському комп'ютері, нові командлети V2 продовжуватимуть працювати (на відміну від старіших командлетів RPS).
