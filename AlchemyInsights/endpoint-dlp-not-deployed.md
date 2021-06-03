---
title: DLP кінцевої точки не розгорнуто на пристрої користувача
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731872"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a>DLP кінцевої точки не розгорнуто на пристрої користувача

Якщо параметр захисту від втрати даних кінцевої точки (DLP) не застосовано до пристрою користувача, переконайтеся, що ви відповідаєте цим вимогам:

- Windows 10 x64 збірки 1809 або пізнішої версії інстальовано на пристрої.
- Інстальовано клієнт захисту від зловмисних програм версії 4.18.2009.7 або новішої.
- Це один **із** таких пристроїв:
    
    - Azure Active Directory приєдналися (Azure AD)
    - Приєднано до гібридної служби Azure AD
    - AAD зареєстровано

- Щоб виконати дії політики, переконайтеся, що microsoft Chromium Edge інстальовано на пристрої кінцевої точки.

Додаткові вимоги до розгортання захисту від втрати даних кінцевої точки див. в цьому [документі.](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)