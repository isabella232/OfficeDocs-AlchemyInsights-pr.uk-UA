---
title: ЗВД політики поради не працюють
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932607"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="e8fce-102">ЗВД політики Підказка питання</span><span class="sxs-lookup"><span data-stu-id="e8fce-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="e8fce-103">**Важливо**: багато SharePoint Online і OneDrive клієнтів, запустіть бізнес-критичних програм від служби, які працюють у фоновому режимі.</span><span class="sxs-lookup"><span data-stu-id="e8fce-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="e8fce-104">До них відносяться міграція вмісту, запобігання втрати даних (ЗВД) і рішення для резервного копіювання.</span><span class="sxs-lookup"><span data-stu-id="e8fce-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="e8fce-105">У ці безпрецедентні часи Ми вживаємо заходів, щоб гарантувати, що служби SharePoint Online та OneDrive залишаються дуже доступними та надійними для користувачів, які залежать від служби, ніж будь-коли в віддалених сценаріях роботи.</span><span class="sxs-lookup"><span data-stu-id="e8fce-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="e8fce-106">На підтримку цієї мети, ми реалізували жорсткі обмеження регулювання на фонових програм (міграція, ЗВД і резервне копіювання рішень) в будні дні вдень.</span><span class="sxs-lookup"><span data-stu-id="e8fce-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="e8fce-107">Ви повинні очікувати, що ці програми будуть досягати дуже обмежену пропускну здатність в ці часи.</span><span class="sxs-lookup"><span data-stu-id="e8fce-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="e8fce-108">Однак під час вечірніх та вихідних годин для регіону служба буде готова обробляти значно більший обсяг запитів від фонових програм.</span><span class="sxs-lookup"><span data-stu-id="e8fce-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="e8fce-109">**ЗВД політики поради**</span><span class="sxs-lookup"><span data-stu-id="e8fce-109">**DLP policy tips**</span></span>

<span data-ttu-id="e8fce-110">Під час використання **звд**політики, користувачі можуть отримувати повідомлення про порушення правил політики **поради**.</span><span class="sxs-lookup"><span data-stu-id="e8fce-110">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="e8fce-111">Адміністратори можуть настроювати політики поради для відображення під час тестування, їх ЗВД політики або коли політики в режимі повного примусового виконання.</span><span class="sxs-lookup"><span data-stu-id="e8fce-111">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="e8fce-112">Щоб настроїти рекомендації політики щодо політики ЗВД у центрі безпеки та комплаєнсу в повному режимі примусового виконання, виконайте такі дії.</span><span class="sxs-lookup"><span data-stu-id="e8fce-112">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="e8fce-113">Переконайтеся, що поради щодо політики **ввімкнено** для правила звд, використовуючи наведені [нижче дії.](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="e8fce-113">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="e8fce-114">Переконайтеся, що ваш **вміст збігається** з тим, що **потрібно** , щоб ініціювати правило, викладену в цій статті [тут](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="e8fce-114">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="e8fce-115">Політики поради відображення в OWA та Outlook.</span><span class="sxs-lookup"><span data-stu-id="e8fce-115">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="e8fce-116">Однак під час використання **Outlook 2013 або новішої версії**, поради політики відображаються лише за певних умов.</span><span class="sxs-lookup"><span data-stu-id="e8fce-116">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="e8fce-117">Тут перераховані умови: [Підтримувані умови для Outlook 2013 або пізнішої версії для відображення поради щодо політики](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span><span class="sxs-lookup"><span data-stu-id="e8fce-117">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span></span>

<span data-ttu-id="e8fce-118">Щоб отримати додаткові відомості про ЗВД політики поради див.: [Показувати політики поради для звд](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips) політики</span><span class="sxs-lookup"><span data-stu-id="e8fce-118">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span></span>
  