---
title: 618 політика спільного доступу до календаря
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/26/2020
ms.locfileid: "44373020"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="ec7ec-102">Політика помилка під час спільного доступу до календаря</span><span class="sxs-lookup"><span data-stu-id="ec7ec-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="ec7ec-103">Виконайте одну з наведених нижче дій відповідно до ситуації.</span><span class="sxs-lookup"><span data-stu-id="ec7ec-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="ec7ec-104">Підключення до Exchange Online за допомогою віддаленого PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ec7ec-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="ec7ec-105">Для отримання додаткових відомостей див. [підключення до Exchange Online за допомогою віддаленого PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="ec7ec-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="ec7ec-106">На локальному сервері, відкрийте оболонку керування Exchange.</span><span class="sxs-lookup"><span data-stu-id="ec7ec-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="ec7ec-107">Визначте політику спільного доступу, призначену для користувача.</span><span class="sxs-lookup"><span data-stu-id="ec7ec-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="ec7ec-108">Для цього виконайте таку команду та запишіть політику, що повертається:</span><span class="sxs-lookup"><span data-stu-id="ec7ec-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="ec7ec-109">Оновіть політику спільного доступу для користувача.</span><span class="sxs-lookup"><span data-stu-id="ec7ec-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="ec7ec-110">Щоб зробити це, виконайте такі дії.</span><span class="sxs-lookup"><span data-stu-id="ec7ec-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="ec7ec-111">Відкрийте Центр адміністрування Exchange.</span><span class="sxs-lookup"><span data-stu-id="ec7ec-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="ec7ec-112">Клацніть **організації**, а потім двічі клацніть політику, призначену користувачу під **окремим спільним доступом**.</span><span class="sxs-lookup"><span data-stu-id="ec7ec-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="ec7ec-113">Це політика, яка була повернена на кроці 2.</span><span class="sxs-lookup"><span data-stu-id="ec7ec-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="ec7ec-114">На сторінці правила спільного доступу виберіть рівень спільного доступу до календаря, який потрібно дозволити у розділі **Укажіть відомості, які потрібно надати спільний доступ**; натисніть кнопку **зберегти**.</span><span class="sxs-lookup"><span data-stu-id="ec7ec-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="ec7ec-115">Щоб отримати додаткові відомості див.: ["політика не дозволяє надання дозволів на цьому рівні один або кілька одержувачів (ів)" помилка, коли користувач намагається надати спільний доступ до календаря](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="ec7ec-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
