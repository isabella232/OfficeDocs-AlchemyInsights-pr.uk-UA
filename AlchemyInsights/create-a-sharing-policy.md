---
title: Створення політики спільного доступу для надання користувачам спільного доступу до календаря користувачам поза межами організації
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 016b915a9e8f7e32d5d393bc47347991866647c7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816293"
---
# <a name="create-a-sharing-policy-to-allow-your-users-to-share-their-calendar-with-people-outside-your-organization"></a><span data-ttu-id="78fe1-102">Створення політики спільного доступу для надання користувачам спільного доступу до календаря користувачам поза межами організації</span><span class="sxs-lookup"><span data-stu-id="78fe1-102">Create a Sharing Policy to allow your users to share their calendar with people outside your organization</span></span>

1. <span data-ttu-id="78fe1-103">З приладної дошки Центру адміністрування Microsoft 365 перейдіть до **Exchange**  >  **адміністратора.**</span><span class="sxs-lookup"><span data-stu-id="78fe1-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="78fe1-104">Перейдіть до **спільного доступу**  >  **до організації.**</span><span class="sxs-lookup"><span data-stu-id="78fe1-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="78fe1-105">У поданні списку в розділі **Окремий спільний доступ** натисніть кнопку **Створити** .</span><span class="sxs-lookup"><span data-stu-id="78fe1-105">In the list view, under **Individual Sharing**, click **New** .</span></span>
4. <span data-ttu-id="78fe1-106">У **новій політиці спільного** доступу введіть зрозуміле ім'я політики спільного доступу в **полі Ім'я політики.**</span><span class="sxs-lookup"><span data-stu-id="78fe1-106">In **new sharing policy**, type a friendly name for the sharing policy in the **Policy name** box.</span></span>
5. <span data-ttu-id="78fe1-107">Натисніть **кнопку Додати,**  щоб визначити правила спільного доступу для політики.</span><span class="sxs-lookup"><span data-stu-id="78fe1-107">Click **Add**  to define the sharing rules for the policy.</span></span>
6. <span data-ttu-id="78fe1-108">У **правилі спільного** доступу виберіть один із наведених нижче параметрів, щоб указати домени, до яких потрібно надати спільний доступ.</span><span class="sxs-lookup"><span data-stu-id="78fe1-108">In **sharing rule**, select one of the following options to specify the domains you want to share with:</span></span>
    - <span data-ttu-id="78fe1-109">**Надання спільного доступу для всіх доменів**</span><span class="sxs-lookup"><span data-stu-id="78fe1-109">**Sharing with all domains**</span></span>
    - <span data-ttu-id="78fe1-110">**Надання спільного доступу для певного домену**</span><span class="sxs-lookup"><span data-stu-id="78fe1-110">**Sharing with a specific domain**</span></span>
8. <span data-ttu-id="78fe1-111">Якщо ви **вибрали варіант Спільний доступ для певного** домену, введіть ім'я домену, якому потрібно надати спільний доступ.</span><span class="sxs-lookup"><span data-stu-id="78fe1-111">If you select **Sharing with a specific domain**, type the name of the domain you want to share with.</span></span> <span data-ttu-id="78fe1-112">Якщо потрібно ввести кілька доменів для цієї політики спільного доступу, збережіть параметри для першого домену, а потім змініть правила спільного доступу, щоб додати більше доменів.</span><span class="sxs-lookup"><span data-stu-id="78fe1-112">If you need to enter more than one domain for this sharing policy, save the settings for the first domain, then edit the sharing rules to add more domains.</span></span>
9. <span data-ttu-id="78fe1-113">Щоб указати відомості, до яких можна надавати спільний доступ, **установіть** прапорець Надати спільний доступ до папки календаря, а потім виберіть один із таких параметрів:</span><span class="sxs-lookup"><span data-stu-id="78fe1-113">To specify the information that can be shared, select the **Share your calendar folder** check box, and then select one of the following options:</span></span>
    - <span data-ttu-id="78fe1-114">**Відомості про зайнятість у календарі лише з часом**</span><span class="sxs-lookup"><span data-stu-id="78fe1-114">**Calendar free/busy information with time only**</span></span>
    - <span data-ttu-id="78fe1-115">**Відомості про зайнятість у календарі з часом, темою та розташуванням**</span><span class="sxs-lookup"><span data-stu-id="78fe1-115">**Calendar free/busy information with time, subject, and location**</span></span>
    - <span data-ttu-id="78fe1-116">**Усі відомості про зустрічі в календарі, включно з часом, темою, розташуванням і посадою**</span><span class="sxs-lookup"><span data-stu-id="78fe1-116">**All calendar appointment information, including time, subject, location and title**</span></span>
11. <span data-ttu-id="78fe1-117">Натисніть **кнопку зберегти,** щоб установити правила для політики спільного доступу.</span><span class="sxs-lookup"><span data-stu-id="78fe1-117">Click **save** to set the rules for the sharing policy.</span></span>
12. <span data-ttu-id="78fe1-118">Щоб установити цю політику спільного доступу як нову політику спільного доступу за замовчуванням для всіх користувачів в організації, установіть прапорець Зробити цю політику моєю політикою спільного **доступу** за замовчуванням.</span><span class="sxs-lookup"><span data-stu-id="78fe1-118">If you want to set this sharing policy as the new default sharing policy for all users in your organization, select the **Make this policy my default sharing policy** check box.</span></span>
13. <span data-ttu-id="78fe1-119">Натисніть **кнопку зберегти,** щоб створити політику спільного доступу.</span><span class="sxs-lookup"><span data-stu-id="78fe1-119">Click **save** to create the sharing policy.</span></span>  

<span data-ttu-id="78fe1-120">**Щоб мати повне розуміння цієї теми, див.:**</span><span class="sxs-lookup"><span data-stu-id="78fe1-120">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="78fe1-121">Створення політики спільного доступу в Exchange Online</span><span class="sxs-lookup"><span data-stu-id="78fe1-121">Create a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/create-a-sharing-policy)
- [<span data-ttu-id="78fe1-122">Застосування політики спільного доступу до поштових скриньок в Exchange Online</span><span class="sxs-lookup"><span data-stu-id="78fe1-122">Apply a sharing policy to mailboxes in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy)
- [<span data-ttu-id="78fe1-123">Змінення, вимкнення або видалення політики спільного доступу в Exchange Online</span><span class="sxs-lookup"><span data-stu-id="78fe1-123">Modify, disable, or remove a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)