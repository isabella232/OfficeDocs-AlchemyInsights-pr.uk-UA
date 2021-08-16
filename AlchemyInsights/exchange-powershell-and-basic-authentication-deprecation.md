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
ms.openlocfilehash: 7b5acf4dd3061c7d9ed23d52a8355865592b9a1d743025fc9300dcda5a18831a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069265"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell і припинення підтримки базової автентифікації

Найновіші відомості про підключення до Exchange Online PowerShell без використання базової автентифікації [див. тут](https://aka.ms/exops-docs). Модуль PowerShell V2 не використовує базову автентифікацію.

Зверніть увагу, що базову автентифікацію все одно потрібно ввімкнути на клієнтському комп'ютері.
У новому модулі PowerShell V2 використовується сучасна автентифікація, щоб установити підключення для ввімкнення всіх командлетів V2 на основі REST. Крім того, можна отримати доступ до старіших командлетів PowerShell (RPS), створивши віддалений сеанс PowerShell. Щоб створити сеанс RPS на комп'ютері з ОС Windows, необхідно ввімкнути базову автентифікацію WinRM на клієнтському комп’ютері, хоча в модулі використовується механізм сучасної автентифікації для автентифікації в службі. Канал базової автентифікації WinRM використовується для транспортування маркерів сучасної автентифікації. Якщо базову автентифікацію WinRM вимкнуто на клієнтському комп'ютері, нові командлети V2 продовжуватимуть працювати (на відміну від старіших командлетів RPS).
