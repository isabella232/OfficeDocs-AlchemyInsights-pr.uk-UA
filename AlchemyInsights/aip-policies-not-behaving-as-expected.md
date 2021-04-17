---
title: 'AIP: політики поведінки не так, як очікувалося'
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
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821648"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="1b379-102">AIP: політики поведінки не так, як очікувалося</span><span class="sxs-lookup"><span data-stu-id="1b379-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="1b379-103">Захист даних в Azure. Політики, які не поводяться належним чином, див. в наведених нижче рекомендаціях щодо різних проблем політики.</span><span class="sxs-lookup"><span data-stu-id="1b379-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="1b379-104">Якщо у вас виникають проблеми з візуальною маркуванням, перевірте, коли застосовуються [візуальні позначення.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)</span><span class="sxs-lookup"><span data-stu-id="1b379-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="1b379-105">Якщо виникають проблеми з автоматичним підписуванням, ознайомтеся зі статтями Як [](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)налаштувати умови для автоматичної та рекомендованої класифікації для захисту даних [в Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) і Який вигляд мають типи відомостей.</span><span class="sxs-lookup"><span data-stu-id="1b379-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="1b379-106">Якщо у вас виникають проблеми з захистом власного файлу або Pfile, перегляньте [конфігурацію файлу API.](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)</span><span class="sxs-lookup"><span data-stu-id="1b379-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="1b379-107">Перевірте, чи використовується ненастроєні вами масштабовані політики: Налаштування політики захисту даних Azure для певних користувачів за допомогою масштабних [політик.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)</span><span class="sxs-lookup"><span data-stu-id="1b379-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="1b379-108">Якщо автоматичне маркування не працює в Outlook під час вкладення документа з підписами, переконайтеся, що DRMEncryptProperty не визначено, як описано в статті Параметри реєстру [IRM для](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)безпеки.</span><span class="sxs-lookup"><span data-stu-id="1b379-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="1b379-109">Якщо проблеми не зникають, збирайте журнали клієнта Azure Information Protection і вкладіть експортовані журнали до цього запиту.</span><span class="sxs-lookup"><span data-stu-id="1b379-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="1b379-110">Відкрийте документ Office або створіть електронний лист у програмі Outlook.</span><span class="sxs-lookup"><span data-stu-id="1b379-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="1b379-111">Натисніть **кнопку Довідка та відгуки щодо** захисту та  >  **чутливості.**</span><span class="sxs-lookup"><span data-stu-id="1b379-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="1b379-112">Натисніть **кнопку Експорт журналів**.</span><span class="sxs-lookup"><span data-stu-id="1b379-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="1b379-113">Збережіть журнали у вибраному розташуванні та вкладіть їх до цього запиту на обслуговування.</span><span class="sxs-lookup"><span data-stu-id="1b379-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="1b379-114">Додаткові ресурси:</span><span class="sxs-lookup"><span data-stu-id="1b379-114">Additional resources:</span></span>

- [<span data-ttu-id="1b379-115">Налаштування мітки для візуальних позначок для захисту даних в Azure</span><span class="sxs-lookup"><span data-stu-id="1b379-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="1b379-116">Перегляд документації для захисту даних в Azure</span><span class="sxs-lookup"><span data-stu-id="1b379-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="1b379-117">Використання міток чутливості в програмах Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="1b379-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

