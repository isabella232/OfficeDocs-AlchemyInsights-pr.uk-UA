---
title: Політики умовного доступу
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002357"
- "4583"
ms.openlocfilehash: 8ce41d007988f2a45f1ded385ae50ac3def97c1b
ms.sourcegitcommit: 9923ce61344e22c4490549b12f65fa2896490b1f
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/01/2020
ms.locfileid: "43100641"
---
# <a name="conditional-access-policies"></a><span data-ttu-id="58d4c-102">Політики умовного доступу</span><span class="sxs-lookup"><span data-stu-id="58d4c-102">Conditional Access policies</span></span>

<span data-ttu-id="58d4c-103">Умовний доступ – це можливість Azure AD застосовувати елементи керування під час доступу до програм у вашому середовищі, відповідно до конкретних умов, а також керувати ними з центрального розташування.</span><span class="sxs-lookup"><span data-stu-id="58d4c-103">Conditional Access is a capability of Azure AD that enables you to enforce controls on the access to apps in your environment, all based on specific conditions and managed from a central location.</span></span>

<span data-ttu-id="58d4c-104">Докладні відомості див. у статті [Умовний доступ Azure AD](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="58d4c-104">Learn more about [Azure AD Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>  

<span data-ttu-id="58d4c-105">**Примітка**. Якщо ваш клієнт створено після 21 жовтня 2019 р. і ви неочікувано отримуєте запит на проведення БФА, ймовірно, у вашому клієнті увімкнено [стандартні параметри безпеки](http://aka.ms/securitydefaults).</span><span class="sxs-lookup"><span data-stu-id="58d4c-105">**Note**: If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](http://aka.ms/securitydefaults) enabled in your tenant.</span></span>

<span data-ttu-id="58d4c-106">**Щоб керувати стандартними параметрами безпеки, зробіть ось що.**</span><span class="sxs-lookup"><span data-stu-id="58d4c-106">**To Manage security defaults**</span></span>

1. <span data-ttu-id="58d4c-107">Увійдіть у [Центр адміністрування](https://go.microsoft.com/fwlink/p/?linkid=834822) за допомогою облікових даних глобального адміністратора.</span><span class="sxs-lookup"><span data-stu-id="58d4c-107">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="58d4c-108">Перейдіть у розділ [Властивості Azure Active Directory](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span><span class="sxs-lookup"><span data-stu-id="58d4c-108">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="58d4c-109">У нижній частині сторінки виберіть **Керування стандартними параметрами безпеки**.</span><span class="sxs-lookup"><span data-stu-id="58d4c-109">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="58d4c-110">Натисніть кнопку **Так**, щоб увімкнути стандартні параметри безпеки, або **Ні**, щоб їх вимкнути.</span><span class="sxs-lookup"><span data-stu-id="58d4c-110">Click **Yes** to enable security defaults or **No** to disable security defaults.</span></span>
