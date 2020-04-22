---
title: Вирішення проблеми, користувач не знайдено в каталозі
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 3b863c5e9962dd29ca2ed41d113041d74830f615
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702759"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="ada60-102">Вирішення проблеми, користувач не знайдено в каталозі</span><span class="sxs-lookup"><span data-stu-id="ada60-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="ada60-103">Якщо користувачі отримують повідомлення про помилку "не вдалося знайти користувача" в каталозі, будь ласка, спробуйте ще раз, коли тип питання є користувачем немає в каталозі.</span><span class="sxs-lookup"><span data-stu-id="ada60-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="ada60-104">Наведені нижче дії можна виконати, щоб вирішити цю проблему.</span><span class="sxs-lookup"><span data-stu-id="ada60-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="ada60-105">Переконайтеся, що обліковий запис, який прийняв запрошення електронною поштою,-це той самий обліковий запис, який використовується для входу пізніше.</span><span class="sxs-lookup"><span data-stu-id="ada60-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="ada60-106">Переконайтеся, що користувач використовує той самий обліковий запис, щоб прийняти запрошення та ввійти на сайт.</span><span class="sxs-lookup"><span data-stu-id="ada60-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="ada60-107">Для отримання додаткових відомостей див. [як керувати псевдоніми для</a> облікового запису Microsoft, щоб керувати входом Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="ada60-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="ada60-108">Перейдіть до кожного сайту (ів), в якому користувач отримує повідомлення про помилку.</span><span class="sxs-lookup"><span data-stu-id="ada60-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="ada60-109">Додайте "/_layouts/15/Car.APX/sorfufforffd = 0" (у подвійних лапках) до кінця URL-адреси сайту.</span><span class="sxs-lookup"><span data-stu-id="ada60-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="ada60-110">Приклад: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="ada60-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="ada60-111">Виберіть користувача зі списку.</span><span class="sxs-lookup"><span data-stu-id="ada60-111">Select the user from the list.</span></span>

- <span data-ttu-id="ada60-112">Натисніть **Видалити дозволи користувача** з стрічки.</span><span class="sxs-lookup"><span data-stu-id="ada60-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="ada60-113">Додайте назад користувача і надішліть запрошення користувачу.</span><span class="sxs-lookup"><span data-stu-id="ada60-113">Add back the User and Resend the invite to the user.</span></span>

