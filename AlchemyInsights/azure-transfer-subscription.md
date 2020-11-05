---
title: Передача права власності на Azure
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
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922174"
---
# <a name="transfer-azure-billing-ownership"></a><span data-ttu-id="4c937-102">Передача права власності на Azure</span><span class="sxs-lookup"><span data-stu-id="4c937-102">Transfer Azure billing ownership</span></span>

<span data-ttu-id="4c937-103">Увійдіть на портал " [Лазурний](https://portal.azure.com/) " як адміністратор облікового запису для виставлення рахунка, який має передплатою, яку потрібно перенести.</span><span class="sxs-lookup"><span data-stu-id="4c937-103">Sign in to the [Azure portal](https://portal.azure.com/) as an administrator of the billing account that has the subscription that you want to transfer.</span></span> <span data-ttu-id="4c937-104">Якщо ви не впевнені, що ви маєте права адміністратора, або якщо вам потрібно визначити, хто є, перегляньте статтю [визначення адміністратора виставлення рахунків](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span><span class="sxs-lookup"><span data-stu-id="4c937-104">If you're not sure if you're and administrator, or if you need to determine who is, see [Determine account billing administrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span></span>

- <span data-ttu-id="4c937-105">Пошук у службі **керування витратами + виставлення рахунків**.</span><span class="sxs-lookup"><span data-stu-id="4c937-105">Search on **Cost Management + Billing**.</span></span>
- <span data-ttu-id="4c937-106">Виберіть пункт **передплати** з області ліворуч.</span><span class="sxs-lookup"><span data-stu-id="4c937-106">Select **Subscriptions** from left pane.</span></span> <span data-ttu-id="4c937-107">Залежно від Access може знадобитися вибрати область виставлення рахунків, а потім **передплачений** або **блакитні передплати**.</span><span class="sxs-lookup"><span data-stu-id="4c937-107">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions**.</span></span>
- <span data-ttu-id="4c937-108">Виберіть пункт **передати право власності на виставлення рахунків** для передплатою, яку потрібно перенести.</span><span class="sxs-lookup"><span data-stu-id="4c937-108">Select **Transfer billing ownership** for the subscription you want to transfer</span></span>
- <span data-ttu-id="4c937-109">Введіть адресу електронної пошти користувача, який є адміністратором виставлення рахунків, який стане новим власником для передплатою, а потім натисніть кнопку **Надіслати запит на перенесення**</span><span class="sxs-lookup"><span data-stu-id="4c937-109">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="4c937-110">Користувач отримує повідомлення електронної пошти з інструкціями, щоб переглянути ваш запит на перенесення.</span><span class="sxs-lookup"><span data-stu-id="4c937-110">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="4c937-111">Щоб затвердити запит на перенесення, користувач вибирає посилання в електронному листі та відповідає інструкціям.</span><span class="sxs-lookup"><span data-stu-id="4c937-111">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="4c937-112">**Примітка**. Якщо ви переносите право власності на ваш обліковий запис для облікового запису користувача в іншому клієнті AZURE AD, усі завдання, які [базуються на рольовій службі керування доступом (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)для керування ресурсами в передплаті, остаточно видалено.</span><span class="sxs-lookup"><span data-stu-id="4c937-112">**Note** : If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="4c937-113">Лише новий власник матиме доступ до керування ресурсами в передплаті.</span><span class="sxs-lookup"><span data-stu-id="4c937-113">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="4c937-114">Докладні відомості наведено в статті [передавання передплатою користувачу в іншому клієнті Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="4c937-114">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="4c937-115">**Рекомендовані документи**</span><span class="sxs-lookup"><span data-stu-id="4c937-115">**Recommended Documents**</span></span>

- [<span data-ttu-id="4c937-116">Передача права власності на «Лазурний» на інший обліковий запис</span><span class="sxs-lookup"><span data-stu-id="4c937-116">Transfer billing ownership of an Azure subscription to another account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [<span data-ttu-id="4c937-117">Про передачу права власності на "Лазурний"</span><span class="sxs-lookup"><span data-stu-id="4c937-117">About transferring billing ownership for an Azure subscription</span></span>](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [<span data-ttu-id="4c937-118">Передача Visual Studio, Партнерська мережа Microsoft (MPN) і оплата під час переходу до dev/Test передплати</span><span class="sxs-lookup"><span data-stu-id="4c937-118">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="4c937-119">Запитання й відповіді про права власності</span><span class="sxs-lookup"><span data-stu-id="4c937-119">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="4c937-120">Усунення проблем із відповідним Передаваннями</span><span class="sxs-lookup"><span data-stu-id="4c937-120">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
