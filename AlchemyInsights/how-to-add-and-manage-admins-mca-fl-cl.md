---
title: Додавання адміністраторів і керування ними
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7424"
ms.openlocfilehash: 25fc25392778ae71ec0553e8d8718ec487738acb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755532"
---
# <a name="how-to-add-and-manage-admins"></a><span data-ttu-id="eb0fe-102">Додавання адміністраторів і керування ними</span><span class="sxs-lookup"><span data-stu-id="eb0fe-102">How to add and manage admins</span></span>

<span data-ttu-id="eb0fe-103">На основі опису проблеми ми знайшли рішення для вас.</span><span class="sxs-lookup"><span data-stu-id="eb0fe-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="eb0fe-104">Більшість клієнтів змогли вирішити свою проблему самостійно, дотримуючись нашої документації.</span><span class="sxs-lookup"><span data-stu-id="eb0fe-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="eb0fe-105">Щоб керувати обліковим записом для виставлення рахунків за угодою клієнтів Microsoft (MCA), можна використовувати різні ролі з потрібним рівнем доступу.</span><span class="sxs-lookup"><span data-stu-id="eb0fe-105">To manage your billing account for a Microsoft Customer Agreement (MCA), you can use different roles with the desired level of access.</span></span> <span data-ttu-id="eb0fe-106">Ці ролі Крім вбудованих ролей служби, які допоможуть вам керувати ресурсами.</span><span class="sxs-lookup"><span data-stu-id="eb0fe-106">These roles are in addition to the built-in Azure service roles which help you control your resources.</span></span>

<span data-ttu-id="eb0fe-107">**Щоб додати ролі виставлення рахунків на порталі Azure, виконайте наведені нижче дії.**</span><span class="sxs-lookup"><span data-stu-id="eb0fe-107">**To add billing roles in the Azure portal:**</span></span>

1. <span data-ttu-id="eb0fe-108">Увійдіть на [портал Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="eb0fe-108">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="eb0fe-109">Знайдіть *керування витратами + виставлення рахунків*.</span><span class="sxs-lookup"><span data-stu-id="eb0fe-109">Search for *Cost Management + Billing*.</span></span>
3. <span data-ttu-id="eb0fe-110">Виберіть елемент керування доступом (IAM) в області, наприклад рахунки для виставлення рахунків, профіль виставлення рахунків або рахунок-фактуру, у якому потрібно надати доступ.</span><span class="sxs-lookup"><span data-stu-id="eb0fe-110">Select Access control (IAM) at a scope such as billing account, billing profile, or invoice section where you want to give access.</span></span>
4. <span data-ttu-id="eb0fe-111">Сторінка керування доступом (IAM) містить список користувачів і груп, призначених кожній ролі для цієї області.</span><span class="sxs-lookup"><span data-stu-id="eb0fe-111">The Access control (IAM) page lists users and groups that are assigned to each role for that scope.</span></span>
5. <span data-ttu-id="eb0fe-112">Щоб надати доступ користувачу, натисніть кнопку **Додати** у верхній частині сторінки.</span><span class="sxs-lookup"><span data-stu-id="eb0fe-112">To give access to a user, select **Add** from the top of the page.</span></span> <span data-ttu-id="eb0fe-113">У розкривному списку *ролей* виберіть роль.</span><span class="sxs-lookup"><span data-stu-id="eb0fe-113">In the *Role* drop-down list, select a role.</span></span> <span data-ttu-id="eb0fe-114">Введіть адресу електронної пошти користувача, якому потрібно надати доступ.</span><span class="sxs-lookup"><span data-stu-id="eb0fe-114">Enter the email address of the user to whom you want to give access.</span></span> <span data-ttu-id="eb0fe-115">Натисніть кнопку **зберегти** , щоб призначити роль.</span><span class="sxs-lookup"><span data-stu-id="eb0fe-115">Select **Save** to assign the role.</span></span>
6. <span data-ttu-id="eb0fe-116">Щоб видалити доступ для користувача, виберіть користувача з призначенням ролей, яке потрібно видалити.</span><span class="sxs-lookup"><span data-stu-id="eb0fe-116">To remove access for a user, select the user with the role assignment you want to remove.</span></span> <span data-ttu-id="eb0fe-117">Натисніть кнопку **Видалити**.</span><span class="sxs-lookup"><span data-stu-id="eb0fe-117">Select **Remove**.</span></span>

<span data-ttu-id="eb0fe-118">**Рекомендовані документи**</span><span class="sxs-lookup"><span data-stu-id="eb0fe-118">**Recommended Documents**</span></span>

- [<span data-ttu-id="eb0fe-119">Визначення ролей для виставлення рахунків</span><span class="sxs-lookup"><span data-stu-id="eb0fe-119">Billing role definitions</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [<span data-ttu-id="eb0fe-120">Ролі та завдання облікового запису для виставлення рахунків</span><span class="sxs-lookup"><span data-stu-id="eb0fe-120">Billing account roles and tasks</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [<span data-ttu-id="eb0fe-121">Початок роботи з обліковим записом для виставлення рахунків MCA</span><span class="sxs-lookup"><span data-stu-id="eb0fe-121">Get started with your MCA billing account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [<span data-ttu-id="eb0fe-122">Перевірка доступу до угоди клієнта Microsoft</span><span class="sxs-lookup"><span data-stu-id="eb0fe-122">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
