---
title: Видалити загублений користувача з локального сервера
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198583"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="e853b-102">Видалити загублений користувача з локального сервера</span><span class="sxs-lookup"><span data-stu-id="e853b-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="e853b-103">Щоб видалити загублений користувача, виконайте такі дії:</span><span class="sxs-lookup"><span data-stu-id="e853b-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="e853b-104">Примусове синхронізації каталогів, слідуючи інструкціям в [тому, що таке Гібридна ідентичність з Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span><span class="sxs-lookup"><span data-stu-id="e853b-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="e853b-105">Щоб перевірити синхронізацію каталогів, подивіться, [що таке Гібридна ідентичність з Active Directory Azure?](https://technet.microsoft.com/library/jj151797.aspx).</span><span class="sxs-lookup"><span data-stu-id="e853b-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="e853b-106">Якщо функція синхронізації належним чином, але видалення об'єкта Active Directory не поширюється на Azure AD, вручну видалити загублений об'єкт за допомогою одного з таких Azure Active Directory модуль для командлети оболонки Windows PowerShell:</span><span class="sxs-lookup"><span data-stu-id="e853b-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="e853b-107">Видалити-MsolContact</span><span class="sxs-lookup"><span data-stu-id="e853b-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="e853b-108">Видалити-MsolGroup</span><span class="sxs-lookup"><span data-stu-id="e853b-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="e853b-109">Видалення MsolUser</span><span class="sxs-lookup"><span data-stu-id="e853b-109">Remove-MsolUser</span></span>

    <span data-ttu-id="e853b-110">Наприклад, щоб видалити загублений ІДЕНТИФІКАТОР користувача john.smith@contoso.com, спочатку створеного за допомогою синхронізації каталогів, запустіть командлет:</span><span class="sxs-lookup"><span data-stu-id="e853b-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="e853b-111">Видалення MsolUser – ім'я користувача John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="e853b-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>