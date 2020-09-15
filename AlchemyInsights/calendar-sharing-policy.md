---
title: Політика спільного доступу до календаря 618
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684251"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="76a8e-102">Помилка політики під час надання спільного доступу до календаря</span><span class="sxs-lookup"><span data-stu-id="76a8e-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="76a8e-103">Виконайте одну з наведених нижче дій відповідно до ситуації.</span><span class="sxs-lookup"><span data-stu-id="76a8e-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="76a8e-104">Підключіться до служби Exchange Online за допомогою віддаленого PowerShell.</span><span class="sxs-lookup"><span data-stu-id="76a8e-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="76a8e-105">Додаткові відомості наведено в статті [підключення до служби Exchange Online за допомогою віддаленого PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="76a8e-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="76a8e-106">На локальному сервері відкрийте оболонку керування Exchange.</span><span class="sxs-lookup"><span data-stu-id="76a8e-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="76a8e-107">Визначте політику спільного доступу, призначену користувачу.</span><span class="sxs-lookup"><span data-stu-id="76a8e-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="76a8e-108">Щоб виконати цю дію, виконайте таку команду та зверніть увагу на те, що політика повернулась:</span><span class="sxs-lookup"><span data-stu-id="76a8e-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="76a8e-109">Оновіть політику спільного доступу для користувача.</span><span class="sxs-lookup"><span data-stu-id="76a8e-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="76a8e-110">Щоб зробити це, виконайте такі дії.</span><span class="sxs-lookup"><span data-stu-id="76a8e-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="76a8e-111">Відкрийте Центр адміністрування Exchange.</span><span class="sxs-lookup"><span data-stu-id="76a8e-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="76a8e-112">Виберіть елемент **організація**, а потім двічі клацніть політику, призначену користувачу під **окремим спільним доступом**.</span><span class="sxs-lookup"><span data-stu-id="76a8e-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="76a8e-113">Це політика, повернуте на кроці 2.</span><span class="sxs-lookup"><span data-stu-id="76a8e-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="76a8e-114">На сторінці правило спільного доступу виберіть рівень спільного доступу до календаря, який потрібно дозволити в розділі **Укажіть відомості, які потрібно надати спільний доступ**. натисніть кнопку **зберегти**.</span><span class="sxs-lookup"><span data-stu-id="76a8e-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="76a8e-115">Для отримання додаткових відомостей див.: ["політика не дає дозволу на надання дозволів на цей рівень до одного або кількох одержувачів" під час спроби користувача надати спільний доступ до календаря](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="76a8e-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
