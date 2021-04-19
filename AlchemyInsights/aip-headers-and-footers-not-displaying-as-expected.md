---
title: 'AIP: колонтитули не відображаються належним чином'
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
- "9002266"
- "4541"
ms.openlocfilehash: 5f50fc1d38618017bca61b4e9290d9893983534e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821720"
---
# <a name="aip-headers-and-footers-not-displaying-as-expected"></a><span data-ttu-id="123b3-102">AIP: колонтитули не відображаються належним чином</span><span class="sxs-lookup"><span data-stu-id="123b3-102">AIP: Headers and footers not displaying as expected</span></span>

<span data-ttu-id="123b3-103">Якщо виникають проблеми з візуальним позначенням, які не відображаються належним чином, перегляньте наведені нижче рекомендації.</span><span class="sxs-lookup"><span data-stu-id="123b3-103">If you are experiencing issues with visual markings not displaying as expected, view the following guidelines:</span></span>

1. <span data-ttu-id="123b3-104">Переконайтеся, що ви перевірили, [коли застосовано візуальні позначення.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)</span><span class="sxs-lookup"><span data-stu-id="123b3-104">Make sure you have reviewed [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="123b3-105">Відомості про маркування Office див. в розділі Коли [служба Office 365](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps#when-office-apps-apply-content-marking-and-encryption)застосовує позначення вмісту та шифрування.</span><span class="sxs-lookup"><span data-stu-id="123b3-105">For Office labeling, review [When Office 365 applies content marking and encryption](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps#when-office-apps-apply-content-marking-and-encryption).</span></span>
3. <span data-ttu-id="123b3-106">Якщо потрібно видалити наявні колонтитули, ознайомтеся зі стосом Видалення колонтитулів з інших рішень [для підписування.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-customizations#remove-headers-and-footers-from-other-labeling-solutions)</span><span class="sxs-lookup"><span data-stu-id="123b3-106">If you want to remove existing headers/footers, review [Remove headers and footers from other labeling solutions](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-customizations#remove-headers-and-footers-from-other-labeling-solutions).</span></span>

<span data-ttu-id="123b3-107">Якщо проблема не зникає, збирайте журнали клієнта Захисту даних Azure і вкладіть експортовані журнали до цього запиту.</span><span class="sxs-lookup"><span data-stu-id="123b3-107">If you are still experiencing the issue, collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

<span data-ttu-id="123b3-108">**Експорт журналів захисту даних в Azure**</span><span class="sxs-lookup"><span data-stu-id="123b3-108">**Export Azure Information Protection logs**</span></span>

1. <span data-ttu-id="123b3-109">Відкрийте документ Office або створіть електронний лист у програмі Outlook.</span><span class="sxs-lookup"><span data-stu-id="123b3-109">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="123b3-110">Натисніть **кнопку Довідка та відгуки щодо** захисту та  >  **чутливості.**</span><span class="sxs-lookup"><span data-stu-id="123b3-110">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="123b3-111">Натисніть **кнопку Експорт журналів**.</span><span class="sxs-lookup"><span data-stu-id="123b3-111">Click **Export Logs**.</span></span>
4. <span data-ttu-id="123b3-112">Збережіть журнали у вибраному розташуванні та вкладіть їх до цього запиту на обслуговування.</span><span class="sxs-lookup"><span data-stu-id="123b3-112">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="123b3-113">Докладні відомості див. в такому:</span><span class="sxs-lookup"><span data-stu-id="123b3-113">For additional information, see:</span></span>

- [<span data-ttu-id="123b3-114">Налаштування мітки для візуальних позначок для захисту даних в Azure</span><span class="sxs-lookup"><span data-stu-id="123b3-114">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="123b3-115">Перегляд документації для захисту даних в Azure</span><span class="sxs-lookup"><span data-stu-id="123b3-115">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="123b3-116">Вимоги до захисту даних в Azure</span><span class="sxs-lookup"><span data-stu-id="123b3-116">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="123b3-117">Короткий посібник із захисту даних в Azure</span><span class="sxs-lookup"><span data-stu-id="123b3-117">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [<span data-ttu-id="123b3-118">Завантаження клієнта Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="123b3-118">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
