---
title: Додаткові відомості про ЗВД питання
ms.author: pebaum
author: pebaum
manager: laurawi
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2447"
- "3200001"
ms.openlocfilehash: 6525cee0555f1ae67b7d4e32445b9a1537d4a804
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932715"
---
# <a name="information-about-dlp-issues"></a><span data-ttu-id="6110c-102">Відомості про ЗВД питання</span><span class="sxs-lookup"><span data-stu-id="6110c-102">Information about DLP issues</span></span>

<span data-ttu-id="6110c-103">**Важливо**: багато SharePoint Online і OneDrive клієнтів, запустіть бізнес-критичних програм від служби, які працюють у фоновому режимі.</span><span class="sxs-lookup"><span data-stu-id="6110c-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="6110c-104">До них відносяться міграція вмісту, запобігання втрати даних (ЗВД) і рішення для резервного копіювання.</span><span class="sxs-lookup"><span data-stu-id="6110c-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="6110c-105">У ці безпрецедентні часи Ми вживаємо заходів, щоб гарантувати, що служби SharePoint Online та OneDrive залишаються дуже доступними та надійними для користувачів, які залежать від служби, ніж будь-коли в віддалених сценаріях роботи.</span><span class="sxs-lookup"><span data-stu-id="6110c-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="6110c-106">На підтримку цієї мети, ми реалізували жорсткі обмеження регулювання на фонових програм (міграція, ЗВД і резервне копіювання рішень) в будні дні вдень.</span><span class="sxs-lookup"><span data-stu-id="6110c-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="6110c-107">Ви повинні очікувати, що ці програми будуть досягати дуже обмежену пропускну здатність в ці часи.</span><span class="sxs-lookup"><span data-stu-id="6110c-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="6110c-108">Однак під час вечірніх та вихідних годин для регіону служба буде готова обробляти значно більший обсяг запитів від фонових програм.</span><span class="sxs-lookup"><span data-stu-id="6110c-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="6110c-109">**Інформація про ЗВД політика**</span><span class="sxs-lookup"><span data-stu-id="6110c-109">**Information on DLP policy**</span></span>

<span data-ttu-id="6110c-110">За допомогою політики ЗВД можна ідентифікувати, контролювати та автоматично захищати конфіденційну інформацію в Office 365.</span><span class="sxs-lookup"><span data-stu-id="6110c-110">With a DLP policy, you can identify, monitor, and automatically protect sensitive information across Office 365.</span></span>

<span data-ttu-id="6110c-111">Будь ласка, відвідайте ці посилання для отримання додаткової інформації:</span><span class="sxs-lookup"><span data-stu-id="6110c-111">Please visit these links for more information:</span></span>

- [<span data-ttu-id="6110c-112">Огляд запобігання втраті даних</span><span class="sxs-lookup"><span data-stu-id="6110c-112">Overview of data loss prevention</span></span>](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies)
- [<span data-ttu-id="6110c-113">Які типи конфіденційних даних шукають</span><span class="sxs-lookup"><span data-stu-id="6110c-113">What the sensitive information types look for</span></span>](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
- [<span data-ttu-id="6110c-114">Створення настроюваного типу даних делікатного характеру</span><span class="sxs-lookup"><span data-stu-id="6110c-114">Create a custom sensitive information type</span></span>](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)
- [<span data-ttu-id="6110c-115">Надсилати сповіщення електронною поштою та показувати поради щодо політики</span><span class="sxs-lookup"><span data-stu-id="6110c-115">Send email notifications and show policy tips</span></span>](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)
- [<span data-ttu-id="6110c-116">Захист файлів SharePoint Online з мітками збереження та ЗВД</span><span class="sxs-lookup"><span data-stu-id="6110c-116">Protect SharePoint Online files with retention labels and DLP</span></span>](https://docs.microsoft.com/office365/securitycompliance/protect-sharepoint-online-files-with-office-365-labels-and-dlp)
- [<span data-ttu-id="6110c-117">ЗВД і Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="6110c-117">DLP and Microsoft Teams</span></span>](https://docs.microsoft.com/office365/securitycompliance/dlp-microsoft-teams)

<span data-ttu-id="6110c-118">Щоб перевірити дані за допомогою вбудованого або настроюваного типу даних делікатного характеру, скористайтеся параметром **Test Type** **у розділі** > **типи конфіденційних**відомостей.</span><span class="sxs-lookup"><span data-stu-id="6110c-118">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="6110c-119">Щоб [отримати додаткові відомості див.](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center)</span><span class="sxs-lookup"><span data-stu-id="6110c-119">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>