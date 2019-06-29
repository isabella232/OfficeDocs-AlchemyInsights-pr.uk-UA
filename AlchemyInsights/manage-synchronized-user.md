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
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="9ca90-102">Не вдалося встановити основна адреса електронної пошти або змінити атрибути користувача</span><span class="sxs-lookup"><span data-stu-id="9ca90-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="9ca90-103">Ввімкненої синхронізації каталогів для вашого середовища деякі атрибути користувача або об'єкт не можна змінити за допомогою Центру адміністрування.</span><span class="sxs-lookup"><span data-stu-id="9ca90-103">If directory synchronization is enabled for your environment some user or object attributes cannot be changed using the Admin Center.</span></span>
<span data-ttu-id="9ca90-104">Повністю керування синхронізовані користувачами та їхніх атрибутів, використовувати ваші місцеві служби active directory користувачі та групи консолі керування (команду adsiedit. msc).</span><span class="sxs-lookup"><span data-stu-id="9ca90-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="9ca90-105">Крім того, ви можете змінити окремих користувачів або атрибутів для синхронізовані користувачів за допомогою оболонки powershell, такі, як показано в ці загальні приклади:</span><span class="sxs-lookup"><span data-stu-id="9ca90-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="9ca90-106">Set-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="9ca90-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="9ca90-107">Set-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Тестового користувача" - Прізвище "Користувач"-посадою «Менеджер»-департамент "Управління Персоналом"</span><span class="sxs-lookup"><span data-stu-id="9ca90-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="9ca90-108">Видалити MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="9ca90-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>