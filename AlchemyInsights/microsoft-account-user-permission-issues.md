---
title: Створення та використання спільної поштової скриньки
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81bf8082198de1c44037291f23c434d06a77f02a
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762421"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="8f0d9-102">Усунення проблем: питання - користувача не знайдено в каталозі</span><span class="sxs-lookup"><span data-stu-id="8f0d9-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="8f0d9-103">Якщо користувачі отримують помилка повідомлення «не вдалося знайти користувача"в каталозі.</span><span class="sxs-lookup"><span data-stu-id="8f0d9-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="8f0d9-104">Будь ласка, спробуйте ще раз де тип питання немає користувача в каталозі.</span><span class="sxs-lookup"><span data-stu-id="8f0d9-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="8f0d9-105">Наступні кроки можна завершити виправлення цієї неполадки.</span><span class="sxs-lookup"><span data-stu-id="8f0d9-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="8f0d9-106">Забезпечити обліковий запис, який прийняв запрошення електронною поштою один обліковий запис, який використовується для входу в пізніше.</span><span class="sxs-lookup"><span data-stu-id="8f0d9-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="8f0d9-107">Переконайтеся, що користувач використовує той самий обліковий запис прийняти запрошення і входу на сайт.</span><span class="sxs-lookup"><span data-stu-id="8f0d9-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="8f0d9-108">Для отримання додаткової інформації див [як керувати псевдоніми для облікового запису Microsoft</a> керувати Office 365 Логін](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="8f0d9-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="8f0d9-109">Знайдіть кожен сайт (и), в якій користувач отримує повідомлення про помилку.</span><span class="sxs-lookup"><span data-stu-id="8f0d9-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="8f0d9-110">Додавання "/ _layouts/15/people.aspx/membershipgroupid=0" (в подвійні лапки) в кінці URL-адреси сайту.</span><span class="sxs-lookup"><span data-stu-id="8f0d9-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="8f0d9-111">Приклад: https://_lT _"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="8f0d9-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="8f0d9-112">Виберіть користувача зі списку.</span><span class="sxs-lookup"><span data-stu-id="8f0d9-112">Select the user from the list.</span></span>

- <span data-ttu-id="8f0d9-113">Натисніть кнопку **Видалити дозволи користувачів** зі стрічки.</span><span class="sxs-lookup"><span data-stu-id="8f0d9-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="8f0d9-114">Додати назад користувача та повторно надіслати запрошення для користувача.</span><span class="sxs-lookup"><span data-stu-id="8f0d9-114">Add back the User and Resend the invite to the user.</span></span>

