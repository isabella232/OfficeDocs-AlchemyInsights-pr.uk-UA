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
ms.openlocfilehash: 5a383bdd17c5fa055c35a923ca36e0e0f6d429e4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/28/2019
ms.locfileid: "35380526"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Не вдалося встановити основна адреса електронної пошти або змінити атрибути користувача

Ввімкненої синхронізації каталогів для вашого середовища деякі атрибути користувача або об'єкт не можна змінити за допомогою Центру адміністрування.
Повністю керування синхронізовані користувачами та їхніх атрибутів, використовувати ваші місцеві служби active directory користувачі та групи консолі керування (команду adsiedit. msc).  

Крім того, ви можете змінити окремих користувачів або атрибутів для синхронізовані користувачів за допомогою оболонки powershell, такі, як показано в ці загальні приклади: 
- Set-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Set-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Тестового користувача" - Прізвище "Користувач"-посадою «Менеджер»-департамент "Управління Персоналом"
- Видалити MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com