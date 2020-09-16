---
title: 'AIP: політики, які не ведуть себе належним чином'
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
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663210"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="28f5a-102">AIP: політики, які не ведуть себе належним чином</span><span class="sxs-lookup"><span data-stu-id="28f5a-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="28f5a-103">Azure захисту інформації: політики не ведуть себе належним чином, ознайомтеся з такими порадами щодо рекомендованих рекомендацій для різних питань політики.</span><span class="sxs-lookup"><span data-stu-id="28f5a-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="28f5a-104">Якщо у вас виникли проблеми з візуальним розміткою, перевірте, [чи застосовуються візуальні позначки](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="28f5a-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="28f5a-105">Якщо у вас виникли проблеми з автоматичним етикетуванням, ознайомтеся з тим, [як настроїти умови для автоматичної та рекомендованої класифікації для служби Azure захисту інформації](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) , а [також про те, які типи конфіденційної інформації шукають](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="28f5a-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="28f5a-106">Якщо у вас виникли проблеми зі службою захисту від рідної та Pfile, перегляньте [КОНФІГУРАЦІЮ API для файлів](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="28f5a-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="28f5a-107">Перевірте, чи ви використовуєте політики, які не настроєно належним чином: [як настроїти політику захисту інформації в Лазур для певних користувачів за допомогою політик рівня](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="28f5a-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="28f5a-108">Якщо автоматичне маркування не працює в Outlook під час приєднання до документа з позначкою, переконайтеся, що DRMEncryptProperty не визначено, як описано тут: [Параметри реєстру IRM для системи безпеки](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="28f5a-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="28f5a-109">Якщо у вас все ще виникають проблеми, Зберіть клієнт для захисту інформації з Azure, а також вкладіть експортовані журнали до цього квитка.</span><span class="sxs-lookup"><span data-stu-id="28f5a-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="28f5a-110">Відкрийте документ Office або створіть новий електронний лист у програмі Outlook.</span><span class="sxs-lookup"><span data-stu-id="28f5a-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="28f5a-111">Виберіть посилання **захист/конфіденційність**  >  **і зворотний зв'язок**.</span><span class="sxs-lookup"><span data-stu-id="28f5a-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="28f5a-112">Натисніть кнопку **експорт журналів**.</span><span class="sxs-lookup"><span data-stu-id="28f5a-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="28f5a-113">Збережіть журнали на своєму виборі розташування та вкладіть їх до цього запиту на обслуговування.</span><span class="sxs-lookup"><span data-stu-id="28f5a-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="28f5a-114">Додаткові ресурси:</span><span class="sxs-lookup"><span data-stu-id="28f5a-114">Additional resources:</span></span>

- [<span data-ttu-id="28f5a-115">Настроювання підпису для візуального маркування для захисту інформації за допомогою Azure</span><span class="sxs-lookup"><span data-stu-id="28f5a-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="28f5a-116">Огляд документації з захисту інформації про Azure</span><span class="sxs-lookup"><span data-stu-id="28f5a-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="28f5a-117">Використання міток чутливості у програмах Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="28f5a-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

