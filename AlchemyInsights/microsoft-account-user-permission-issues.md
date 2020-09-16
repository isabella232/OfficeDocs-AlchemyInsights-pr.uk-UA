---
title: Виправлення неполадок із проблемою – користувач не знайдено в каталозі
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725428"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="69ade-102">Виправлення неполадок із проблемою – користувач не знайдено в каталозі</span><span class="sxs-lookup"><span data-stu-id="69ade-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="69ade-103">Якщо користувачі отримують повідомлення про помилку "користувач не може знайти" в каталозі, спробуйте ще раз, коли тип проблеми – користувач, який не належить до каталогу.</span><span class="sxs-lookup"><span data-stu-id="69ade-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="69ade-104">Щоб вирішити цю проблему, можна виконати наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="69ade-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="69ade-105">Переконайтеся, що обліковий запис, який прийняв запрошення на повідомлення електронної пошти, – це той самий обліковий запис, який використовується для входу в пізнішу версію.</span><span class="sxs-lookup"><span data-stu-id="69ade-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="69ade-106">Переконайтеся, що користувач використовує той самий обліковий запис, щоб прийняти запрошення та ввійти на сайт.</span><span class="sxs-lookup"><span data-stu-id="69ade-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="69ade-107">Щоб отримати докладні відомості, Дізнайтеся, [як керувати псевдонімами для облікового запису Microsoft, </a> щоб керувати входом до служби Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="69ade-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="69ade-108">Перейдіть до кожного веб-сайту, у якому користувач отримує повідомлення про помилку.</span><span class="sxs-lookup"><span data-stu-id="69ade-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="69ade-109">Add ("/_layouts/15/Peopl.aspx/membershippid = 0" (у межах двох лапок) до кінця URL-адреси сайту.</span><span class="sxs-lookup"><span data-stu-id="69ade-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="69ade-110">Приклад: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="69ade-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="69ade-111">Виберіть користувача зі списку.</span><span class="sxs-lookup"><span data-stu-id="69ade-111">Select the user from the list.</span></span>

- <span data-ttu-id="69ade-112">Натисніть кнопку **Видалити дозволи користувача** на стрічці.</span><span class="sxs-lookup"><span data-stu-id="69ade-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="69ade-113">Додайте назад користувача та надішліть запрошення до користувача.</span><span class="sxs-lookup"><span data-stu-id="69ade-113">Add back the User and Resend the invite to the user.</span></span>

