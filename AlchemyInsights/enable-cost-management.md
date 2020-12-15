---
title: Увімкнення керування витратами
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678776"
---
# <a name="enable-cost-management"></a><span data-ttu-id="22290-102">Увімкнення керування витратами</span><span class="sxs-lookup"><span data-stu-id="22290-102">Enable cost management</span></span>

<span data-ttu-id="22290-103">**Що означає "витрати відключені для організації"?**</span><span class="sxs-lookup"><span data-stu-id="22290-103">**What does 'costs are disabled for your organization' mean?**</span></span>

<span data-ttu-id="22290-104">Організації за допомогою корпоративної угоди (EA) або облікових записів Microsoft для клієнтів (MCA) можуть забороняти доступ до відомостей про витрати та цінової інформації.</span><span class="sxs-lookup"><span data-stu-id="22290-104">Organizations using Enterprise Agreement (EA) or Microsoft Customer Agreement (MCA) accounts can disable access to cost information and pricing information.</span></span>

<span data-ttu-id="22290-105">Після входу на портал Azure, вони можуть використовувати API для виставлення рахунків для програмного отримання рахунків-фактур (після того, як вони ввімкнув) і відомості про використання.</span><span class="sxs-lookup"><span data-stu-id="22290-105">After logging in to Azure portal, they can use the Billing APIs to programmatically get invoices (once opted-in) and usage details.</span></span>

<span data-ttu-id="22290-106">**Надання іншим користувачам доступу до рахунків-фактур**</span><span class="sxs-lookup"><span data-stu-id="22290-106">**How to allow additional users to access invoices**</span></span>

1. <span data-ttu-id="22290-107">Перейдіть на сторінку з відповідними **передплатою** на порталі Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="22290-107">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="22290-108">Виберіть пункт **рахунки-фактури** , а потім – **доступ до рахунків-фактур**.</span><span class="sxs-lookup"><span data-stu-id="22290-108">Select **Invoices** and then **Access to invoices**.</span></span>
3. <span data-ttu-id="22290-109">Увімкніть доступ, а потім збережіть зміни, щоб дозволити користувачам використовувати ролі на основі передплатою для завантаження рахунків-фактур.</span><span class="sxs-lookup"><span data-stu-id="22290-109">Turn on the access, followed by saving the changes, to allow users in subscription-scoped roles to download invoices.</span></span>

> [!NOTE]
> <span data-ttu-id="22290-110">Адміністратор облікового запису може також настроїти для надсилання рахунків-фактур електронною поштою.</span><span class="sxs-lookup"><span data-stu-id="22290-110">The Account Administrator can also configure to have invoices sent via email.</span></span> <span data-ttu-id="22290-111">Щоб дізнатися більше, перегляньте статтю [отримання рахунка-фактури в електронному листі](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span><span class="sxs-lookup"><span data-stu-id="22290-111">To learn more, see [Get your invoice in email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span></span>

<span data-ttu-id="22290-112">**Додавання користувачів до ролі невізуального рахунка**</span><span class="sxs-lookup"><span data-stu-id="22290-112">**How to add users to the Billing Reader role**</span></span>

1. <span data-ttu-id="22290-113">Перейдіть на сторінку з відповідними **передплатою** на порталі Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="22290-113">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="22290-114">Виберіть **елемент керування доступом (IAM)** , а потім натисніть кнопку **Додати**.</span><span class="sxs-lookup"><span data-stu-id="22290-114">Select **Access control (IAM)** and then click **Add**.</span></span>
3. <span data-ttu-id="22290-115">Виберіть елемент **невізуальний пристрій для виставлення рахунків** на сторінці **Виберіть роль** .</span><span class="sxs-lookup"><span data-stu-id="22290-115">Choose **Billing Reader** in the **Select a role** page.</span></span>
4. <span data-ttu-id="22290-116">Введіть повідомлення електронної пошти користувача, якого потрібно запросити, а потім натисніть кнопку **OK** , щоб надіслати запрошення.</span><span class="sxs-lookup"><span data-stu-id="22290-116">Type the email of the user you want to invite, and then click **OK** to send the invitation.</span></span>
5. <span data-ttu-id="22290-117">Виконайте вказівки, наведені в запрошенні електронної пошти, щоб увійти в систему як невізуальний пристрій для виставлення рахунків.</span><span class="sxs-lookup"><span data-stu-id="22290-117">Follow instructions provided in the invite email to log in as a billing reader.</span></span> <span data-ttu-id="22290-118">Докладні відомості наведено в статті [надання доступу до рахунків](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span><span class="sxs-lookup"><span data-stu-id="22290-118">For more information, see [Grant access to Billing](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span></span>

<span data-ttu-id="22290-119">**Рекомендовані документи**</span><span class="sxs-lookup"><span data-stu-id="22290-119">**Recommended documents**</span></span>

- [<span data-ttu-id="22290-120">Увімкнення подання "да" та "Ао" за допомогою порталу EA</span><span class="sxs-lookup"><span data-stu-id="22290-120">Enable DA and AO views via EA portal</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [<span data-ttu-id="22290-121">Витрати, включені в керування витратами</span><span class="sxs-lookup"><span data-stu-id="22290-121">Costs included in Cost Management</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [<span data-ttu-id="22290-122">Підтримувані пропозиції Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="22290-122">Supported Microsoft Azure Offers</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [<span data-ttu-id="22290-123">Перевірка витрат у аналізі витрат</span><span class="sxs-lookup"><span data-stu-id="22290-123">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [<span data-ttu-id="22290-124">Надання доступу до відомостей для виставлення рахунків</span><span class="sxs-lookup"><span data-stu-id="22290-124">Provide access to billing information</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="22290-125">Перевірка доступу до угоди клієнта Microsoft</span><span class="sxs-lookup"><span data-stu-id="22290-125">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






