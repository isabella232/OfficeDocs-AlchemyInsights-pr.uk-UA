---
title: Сучасний обліковий запис електронної пошти Azure
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
- "9003801"
- "6866"
ms.openlocfilehash: 4df8c49880fe638c1659f76edc0905532d091e45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820847"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="243df-102">Електронна пошта для виводу з облікового запису в Azure</span><span class="sxs-lookup"><span data-stu-id="243df-102">Email invoicing in Azure</span></span>

<span data-ttu-id="243df-103">Щоб оновити параметри рахунка-фактури, потрібно мати роль власника або власника в профілі виставлення рахунків або обліковому записі для виставлення рахунків.</span><span class="sxs-lookup"><span data-stu-id="243df-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="243df-104">Коли ви погодитесь на вхід, усі користувачі з ролями власника, власника, читачів і керівника рахунків у профілі виставлення рахунків отримають свій рахунок електронною поштою.</span><span class="sxs-lookup"><span data-stu-id="243df-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="243df-105">Увійдіть [на портал Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="243df-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="243df-106">Введіть у пошуку **Керування витратами + виставлення рахунків**.</span><span class="sxs-lookup"><span data-stu-id="243df-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="243df-107">У **лівій** частині виберіть Рахунки-фактури, а потім **у** верхній частині сторінки виберіть Рахунок-фактура електронною поштою.</span><span class="sxs-lookup"><span data-stu-id="243df-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="243df-108">Якщо у вас кілька профілів виставлення рахунків, виберіть профіль виставлення рахунків і натисніть **кнопку Увійдіть.**</span><span class="sxs-lookup"><span data-stu-id="243df-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="243df-109">Натисніть **кнопку Оновити**.</span><span class="sxs-lookup"><span data-stu-id="243df-109">Select **Update**.</span></span>
6. <span data-ttu-id="243df-110">Якщо у вас кілька профілів виставлення рахунків, виберіть профіль виставлення рахунків і натисніть **кнопку Увійдіть.**</span><span class="sxs-lookup"><span data-stu-id="243df-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="243df-111">Ви надаєте іншим користувачам доступ до перегляду, завантаження та оплати рахунків, призначивши їм роль диспетчера рахунків для профілю виставлення рахунків MCA або MPA.</span><span class="sxs-lookup"><span data-stu-id="243df-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="243df-112">Якщо ви вирішили отримати рахунок-фактуру електронною поштою, користувачі також отримуватиме рахунки електронною поштою.</span><span class="sxs-lookup"><span data-stu-id="243df-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="243df-113">Увійдіть [на портал Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="243df-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="243df-114">Введіть у пошуку **Керування витратами + виставлення рахунків**.</span><span class="sxs-lookup"><span data-stu-id="243df-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="243df-115">У **лівій частині** виберіть Профілі виставлення рахунків.</span><span class="sxs-lookup"><span data-stu-id="243df-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="243df-116">Зі списку профілів виставлення рахунків виберіть профіль виставлення рахунків, для якого потрібно призначити роль диспетчера рахунків.</span><span class="sxs-lookup"><span data-stu-id="243df-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="243df-117">У **лівій частині** виберіть елемент Керування доступом (IAM), а потім натисніть кнопку **Додати** у верхній частині сторінки.</span><span class="sxs-lookup"><span data-stu-id="243df-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="243df-118">У розкривному списку Роль виберіть Диспетчер рахунків.</span><span class="sxs-lookup"><span data-stu-id="243df-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="243df-119">Введіть адресу електронної пошти користувача, щоб надати доступ.</span><span class="sxs-lookup"><span data-stu-id="243df-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="243df-120">Натисніть **кнопку Зберегти,** щоб призначити роль.</span><span class="sxs-lookup"><span data-stu-id="243df-120">Select **Save** to assign the role.</span></span>
