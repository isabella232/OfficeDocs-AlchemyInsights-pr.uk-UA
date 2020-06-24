---
title: Створення політики спільного доступу для користувачів, які дають змогу користувачам обмінюватися календарем із людьми за межами вашої організації
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: cb2c0af55f4f8833709b6952d3a6e2ac258ce5fc
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862212"
---
# <a name="create-a-sharing-policy-to-allow-your-users-to-share-their-calendar-with-people-outside-your-organization"></a><span data-ttu-id="279d2-102">Створення політики спільного доступу для користувачів, які дають змогу користувачам обмінюватися календарем із людьми за межами вашої організації</span><span class="sxs-lookup"><span data-stu-id="279d2-102">Create a Sharing Policy to allow your users to share their calendar with people outside your organization</span></span>

1. <span data-ttu-id="279d2-103">З інформаційної панелі центру адміністрування Microsoft 365 перейдіть до **адміністратора**  >  **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="279d2-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="279d2-104">Перейдіть до **organization**  >  **спільного доступу**до організації.</span><span class="sxs-lookup"><span data-stu-id="279d2-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="279d2-105">У поданні списку в розділі **індивідуальний спільний доступ**виберіть пункт **створити** .</span><span class="sxs-lookup"><span data-stu-id="279d2-105">In the list view, under **Individual Sharing**, click **New** .</span></span>
4. <span data-ttu-id="279d2-106">В області " **нова політика спільного доступу**" Введіть зрозуміле ім'я політики спільного доступу в полі **ім'я політики** .</span><span class="sxs-lookup"><span data-stu-id="279d2-106">In **new sharing policy**, type a friendly name for the sharing policy in the **Policy name** box.</span></span>
5. <span data-ttu-id="279d2-107">Натисніть кнопку **Додати** , щоб визначити правила спільного використання політики.</span><span class="sxs-lookup"><span data-stu-id="279d2-107">Click **Add**  to define the sharing rules for the policy.</span></span>
6. <span data-ttu-id="279d2-108">У **правилі спільного доступу**виберіть один із таких параметрів, щоб указати домени, з якими потрібно надати спільний доступ:</span><span class="sxs-lookup"><span data-stu-id="279d2-108">In **sharing rule**, select one of the following options to specify the domains you want to share with:</span></span>
    - <span data-ttu-id="279d2-109">**Обмін з усіма доменами**</span><span class="sxs-lookup"><span data-stu-id="279d2-109">**Sharing with all domains**</span></span>
    - <span data-ttu-id="279d2-110">**Спільне використання з певним доменом**</span><span class="sxs-lookup"><span data-stu-id="279d2-110">**Sharing with a specific domain**</span></span>
8. <span data-ttu-id="279d2-111">Якщо вибрати **спільний доступ до певного домену**, введіть ім'я домену, з яким потрібно надати спільний доступ.</span><span class="sxs-lookup"><span data-stu-id="279d2-111">If you select **Sharing with a specific domain**, type the name of the domain you want to share with.</span></span> <span data-ttu-id="279d2-112">Якщо потрібно ввести більше одного домену для цієї політики спільного використання, збережіть параметри для першого домену, а потім відредагуйте правила спільного доступу, щоб додати інші домени.</span><span class="sxs-lookup"><span data-stu-id="279d2-112">If you need to enter more than one domain for this sharing policy, save the settings for the first domain, then edit the sharing rules to add more domains.</span></span>
9. <span data-ttu-id="279d2-113">Щоб указати відомості, які можна спільно використовувати, установіть прапорець **спільний доступ до папки Календар** і виберіть один із таких параметрів:</span><span class="sxs-lookup"><span data-stu-id="279d2-113">To specify the information that can be shared, select the **Share your calendar folder** check box, and then select one of the following options:</span></span>
    - <span data-ttu-id="279d2-114">**Календар відомості про зайнятість лише з часом**</span><span class="sxs-lookup"><span data-stu-id="279d2-114">**Calendar free/busy information with time only**</span></span>
    - <span data-ttu-id="279d2-115">**Календар відомості про зайнятість із часом, темою та розташуванням**</span><span class="sxs-lookup"><span data-stu-id="279d2-115">**Calendar free/busy information with time, subject, and location**</span></span>
    - <span data-ttu-id="279d2-116">**Усі відомості про призначення календаря, включно з часом, предметом, розташуванням і заголовком**</span><span class="sxs-lookup"><span data-stu-id="279d2-116">**All calendar appointment information, including time, subject, location and title**</span></span>
11. <span data-ttu-id="279d2-117">Натисніть кнопку **зберегти** , щоб установити правила для політики спільного доступу.</span><span class="sxs-lookup"><span data-stu-id="279d2-117">Click **save** to set the rules for the sharing policy.</span></span>
12. <span data-ttu-id="279d2-118">Якщо потрібно встановити цю політику спільного доступу як нову політику спільного використання за промовчанням для всіх користувачів організації, установіть прапорець **зробити цю політику типовою політикою спільного використання** .</span><span class="sxs-lookup"><span data-stu-id="279d2-118">If you want to set this sharing policy as the new default sharing policy for all users in your organization, select the **Make this policy my default sharing policy** check box.</span></span>
13. <span data-ttu-id="279d2-119">Натисніть кнопку **зберегти** , щоб створити політику спільного доступу.</span><span class="sxs-lookup"><span data-stu-id="279d2-119">Click **save** to create the sharing policy.</span></span>  

<span data-ttu-id="279d2-120">**Для повного розуміння цієї теми, будь ласка, прочитайте:**</span><span class="sxs-lookup"><span data-stu-id="279d2-120">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="279d2-121">Створення політики спільного доступу в Exchange Online</span><span class="sxs-lookup"><span data-stu-id="279d2-121">Create a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/create-a-sharing-policy)
- [<span data-ttu-id="279d2-122">Застосування політики спільного доступу до поштових скриньок у Exchange Online</span><span class="sxs-lookup"><span data-stu-id="279d2-122">Apply a sharing policy to mailboxes in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy)
- [<span data-ttu-id="279d2-123">Змінення, вимкнення або видалення політики спільного доступу в Exchange Online</span><span class="sxs-lookup"><span data-stu-id="279d2-123">Modify, disable, or remove a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)