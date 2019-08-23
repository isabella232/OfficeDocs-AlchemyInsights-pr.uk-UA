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
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="fb196-102">Не вдалося встановити основна адреса електронної пошти або змінити атрибути користувача</span><span class="sxs-lookup"><span data-stu-id="fb196-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="fb196-103">Ввімкненої синхронізації каталогів для вашого середовища, деякі атрибути користувача або об'єкт не можна змінити за допомогою Центру адміністрування Microsoft Outlook 365.</span><span class="sxs-lookup"><span data-stu-id="fb196-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="fb196-104">Повністю керування синхронізовані користувачами та їхніх атрибутів, використовувати ваші місцеві служби active directory користувачі та групи консолі керування (команду adsiedit. msc).</span><span class="sxs-lookup"><span data-stu-id="fb196-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="fb196-105">Крім того, ви можете змінити окремих користувачів або атрибутів для синхронізовані користувачів за допомогою оболонки powershell, такі, як показано в ці загальні приклади:</span><span class="sxs-lookup"><span data-stu-id="fb196-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="fb196-106">Set-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="fb196-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="fb196-107">Set-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Тестового користувача" - Прізвище "Користувач"-посадою «Менеджер»-департамент "Управління Персоналом"</span><span class="sxs-lookup"><span data-stu-id="fb196-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="fb196-108">Видалити MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="fb196-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>