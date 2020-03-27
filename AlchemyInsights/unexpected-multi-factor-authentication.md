---
title: Неочікувана багатофакторна автентифікація
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ''
ms.custom:
- "1300007"
- "4372"
ms.openlocfilehash: 8a912b32dee23e8c6eae0ad7bc72228d49ceeb92
ms.sourcegitcommit: 4f7ff981bbb3a98663cd164d0a10bb082cdf7ec9
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/25/2020
ms.locfileid: "42946850"
---
# <a name="unexpected-multi-factor-authentication"></a><span data-ttu-id="b5422-102">Неочікувана багатофакторна автентифікація</span><span class="sxs-lookup"><span data-stu-id="b5422-102">Unexpected multi-factor authentication</span></span>

<span data-ttu-id="b5422-103">Якщо ваш клієнт створено після 21 жовтня 2019 р. і ви неочікувано отримуєте запит на проведення БФА, ймовірно, у вашому клієнті увімкнено [стандартні параметри безпеки](http://aka.ms/securitydefaults).</span><span class="sxs-lookup"><span data-stu-id="b5422-103">If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](http://aka.ms/securitydefaults) enabled in your tenant.</span></span> 

<span data-ttu-id="b5422-104">Щоб керувати стандартними параметрами безпеки, зробіть ось що.</span><span class="sxs-lookup"><span data-stu-id="b5422-104">To Manage security defaults:</span></span>

1. <span data-ttu-id="b5422-105">Увійдіть у [Центр адміністрування](https://go.microsoft.com/fwlink/p/?linkid=834822) за допомогою облікових даних глобального адміністратора.</span><span class="sxs-lookup"><span data-stu-id="b5422-105">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="b5422-106">Перейдіть у розділ [Властивості Azure Active Directory](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span><span class="sxs-lookup"><span data-stu-id="b5422-106">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="b5422-107">У нижній частині сторінки виберіть **Керування стандартними параметрами безпеки**.</span><span class="sxs-lookup"><span data-stu-id="b5422-107">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="b5422-108">Натисніть кнопку **Так**, щоб увімкнути стандартні параметри безпеки, або **Ні**, щоб їх вимкнути.</span><span class="sxs-lookup"><span data-stu-id="b5422-108">Click **Yes** to enable security defaults and **No** to disable security defaults.</span></span>
