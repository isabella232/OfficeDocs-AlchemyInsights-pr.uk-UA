---
title: Керувати синхронізованого користувача
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36542038"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Не вдалося встановити основна адреса електронної пошти або змінити атрибути користувача

Ввімкненої синхронізації каталогів для вашого середовища, деякі атрибути користувача або об'єкт не можна змінити за допомогою Центру адміністрування Microsoft Outlook 365.

Повністю керування синхронізовані користувачами та їхніх атрибутів, використовувати ваші місцеві служби active directory користувачі та групи консолі керування (команду adsiedit. msc).  

Крім того, ви можете змінити окремих користувачів або атрибутів для синхронізовані користувачів за допомогою оболонки powershell, такі, як показано в ці загальні приклади: 
- Set-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Set-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Тестового користувача" - Прізвище "Користувач"-посадою «Менеджер»-департамент "Управління Персоналом"
- Видалити MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com