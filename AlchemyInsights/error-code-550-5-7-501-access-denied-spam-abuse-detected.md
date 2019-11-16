---
title: Помилка з кодом 550 5.7.501 доступу заборонено, виявлено порушення спаму
ms.author: chrisda
author: chrisda
ms.date: 6/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "351"
- "3100015"
ms.assetid: 3105905c-e7a0-42a7-9c5a-61dc56a1d6fc
ms.openlocfilehash: 545cab07cc7c49def849be20bb6363da228a5393
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 11/15/2019
ms.locfileid: "36740162"
---
# <a name="550-57501-access-denied-spam-abuse-detected"></a><span data-ttu-id="85d91-102">550 5.7.501 доступ заборонено, виявлено порушення спаму</span><span class="sxs-lookup"><span data-stu-id="85d91-102">550 5.7.501 Access denied, spam abuse detected</span></span>

<span data-ttu-id="85d91-103">Зазвичай це повідомлення виникає, коли користувачі надсилають повідомлення електронної пошти з IP-адрес за допомогою початкового домену *. onmicrosoft.com* , який призначається для нових орендарів у Office 365.</span><span class="sxs-lookup"><span data-stu-id="85d91-103">Typically, this message occurs when users send email messages from IP addresses using the initial *.onmicrosoft.com* domain that's assigned to new tenants in Office 365.</span></span> <span data-ttu-id="85d91-104">Найпростіший спосіб вирішити цю проблему:</span><span class="sxs-lookup"><span data-stu-id="85d91-104">The easiest way to resolve this problem is to:</span></span>

1. <span data-ttu-id="85d91-105">[Додайте домен до свого клієнта](https://docs.microsoft.com//office365/admin/setup/add-domain).</span><span class="sxs-lookup"><span data-stu-id="85d91-105">[Add a domain to your tenant](https://docs.microsoft.com//office365/admin/setup/add-domain).</span></span>

2. <span data-ttu-id="85d91-106">[Змініть основну адресу електронної пошти користувачів](https://docs.microsoft.com//office365/admin/add-users/change-a-user-name-and-email-address) на новий користувацький домен, який ви щойно додали.</span><span class="sxs-lookup"><span data-stu-id="85d91-106">[Change your users' primary email address](https://docs.microsoft.com//office365/admin/add-users/change-a-user-name-and-email-address) to the new custom domain you just added.</span></span>
