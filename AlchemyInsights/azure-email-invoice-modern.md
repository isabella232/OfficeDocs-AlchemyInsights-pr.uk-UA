---
title: Сучасне виставлення рахунка за електронною поштою
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003801"
- "6866"
ms.openlocfilehash: 65df6091a97d4937379ded384a78b5d07aa76e42
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922148"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="e2e09-102">Виставлення рахунка електронною поштою в Лазур</span><span class="sxs-lookup"><span data-stu-id="e2e09-102">Email invoicing in Azure</span></span>

<span data-ttu-id="e2e09-103">Щоб оновити параметри рахунка-фактури, потрібно мати власника або роль вкладника в профілі виставлення рахунків або його рахунок для виставлення рахунків.</span><span class="sxs-lookup"><span data-stu-id="e2e09-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="e2e09-104">Після того як ви вибрали, усі користувачі зі своїми ролями, вкладником, читачами та рахунком-фактурою, а також відповідно до профілю виставлення рахунків, отримають його рахунок-фактуру в електронній пошті.</span><span class="sxs-lookup"><span data-stu-id="e2e09-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="e2e09-105">Увійдіть на [портал Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="e2e09-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="e2e09-106">Знайдіть **керування витратами + виставлення рахунків**.</span><span class="sxs-lookup"><span data-stu-id="e2e09-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="e2e09-107">У лівій частині сторінки виберіть пункт **рахунки-фактури** , а потім виберіть пункт **рахунок електронної пошти** зі списку.</span><span class="sxs-lookup"><span data-stu-id="e2e09-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="e2e09-108">Якщо у вас є кілька профілів виставлення рахунків, виберіть профіль виставлення рахунка, а потім натисніть кнопку **Увімкнути**.</span><span class="sxs-lookup"><span data-stu-id="e2e09-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="e2e09-109">Натисніть кнопку **оновити**.</span><span class="sxs-lookup"><span data-stu-id="e2e09-109">Select **Update**.</span></span>
6. <span data-ttu-id="e2e09-110">Якщо у вас є кілька профілів виставлення рахунків, виберіть профіль виставлення рахунка, а потім натисніть кнопку **Увімкнути**.</span><span class="sxs-lookup"><span data-stu-id="e2e09-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="e2e09-111">Ви даєте іншим користувачам доступ до перегляду, завантаження та виплати рахунків-фактур, призначаючи їм роль диспетчера рахунків для виставлення рахунків MCA або MPA.</span><span class="sxs-lookup"><span data-stu-id="e2e09-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="e2e09-112">Якщо ви вирішили отримати рахунок-фактуру в електронному листі, користувачі також отримують рахунки-фактури в електронній пошті.</span><span class="sxs-lookup"><span data-stu-id="e2e09-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="e2e09-113">Увійдіть на [портал Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="e2e09-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="e2e09-114">Знайдіть **керування витратами + виставлення рахунків**.</span><span class="sxs-lookup"><span data-stu-id="e2e09-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="e2e09-115">Вибір **профілів виставлення рахунків** із лівого боку.</span><span class="sxs-lookup"><span data-stu-id="e2e09-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="e2e09-116">У списку профілі для виставлення рахунків виберіть профіль виставлення рахунка, для якого потрібно призначити роль диспетчера рахунків-фактур.</span><span class="sxs-lookup"><span data-stu-id="e2e09-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="e2e09-117">Виберіть **елемент керування доступом (IAM)** ліворуч, а потім у верхній частині сторінки виберіть пункт **Додати** .</span><span class="sxs-lookup"><span data-stu-id="e2e09-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="e2e09-118">У розкривному списку ролей виберіть елемент **Диспетчер рахунків**.</span><span class="sxs-lookup"><span data-stu-id="e2e09-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="e2e09-119">Введіть адресу електронної пошти користувача, щоб надати доступ.</span><span class="sxs-lookup"><span data-stu-id="e2e09-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="e2e09-120">Натисніть кнопку **зберегти** , щоб призначити роль.</span><span class="sxs-lookup"><span data-stu-id="e2e09-120">Select **Save** to assign the role.</span></span>
