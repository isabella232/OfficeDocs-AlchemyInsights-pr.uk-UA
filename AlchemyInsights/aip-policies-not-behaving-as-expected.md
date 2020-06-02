---
title: 'AIP: політики, не поведінки належним чином'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 527556fcb02525eb88ea992c38a2ddfcba6f9453
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506579"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="d780c-102">AIP: політики, не поведінки належним чином</span><span class="sxs-lookup"><span data-stu-id="d780c-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="d780c-103">Відомості про захист Azure: політики не поводяться належним чином, перегляньте наведені нижче рекомендації щодо рекомендацій щодо різних питань політики:</span><span class="sxs-lookup"><span data-stu-id="d780c-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="d780c-104">Якщо у вас виникли проблеми з візуальними відмітками, будь ласка, перегляньте, [коли застосовуються візуальні позначки](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="d780c-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="d780c-105">Якщо у вас виникли проблеми з автоматичним етикеткуванням, будь ласка, перегляньте, [як налаштувати умови для автоматичної та рекомендованою класифікації для захисту інформації Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) та для [яких типів конфіденційних даних шукати](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="d780c-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="d780c-106">Якщо у вас виникли проблеми з рідним/Pfile захист, будь ласка, перевірте [Конфігурація файлу API](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="d780c-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="d780c-107">Перевірте, якщо використовуються політики в області, які не настроєно належним чином: [Настроювання політики захисту даних Azure для певних користувачів за допомогою політики в](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)області.</span><span class="sxs-lookup"><span data-stu-id="d780c-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="d780c-108">Якщо автоматичне позначення не працює для Outlook під час підключення документа з міткою, переконайтеся, що DRMEncryptProperty не визначено, як описано тут: [Параметри реєстру IRM для безпеки](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="d780c-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="d780c-109">Якщо ви все ще зіткнулися з проблемами, будь ласка, збирайте журнали клієнт захисту інформації Azure і Прикріпіть експортовані журнали до цього квитка.</span><span class="sxs-lookup"><span data-stu-id="d780c-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="d780c-110">Відкрийте документ Office або створіть новий електронний лист у програмі Outlook.</span><span class="sxs-lookup"><span data-stu-id="d780c-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="d780c-111">Натисніть кнопку **захист/чутливість**  >  **Довідка та зворотній зв'язок**.</span><span class="sxs-lookup"><span data-stu-id="d780c-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="d780c-112">Натисніть кнопку **експортувати журнали**.</span><span class="sxs-lookup"><span data-stu-id="d780c-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="d780c-113">Збережіть журнали на ваш вибір місця розташування та Прикріпіть їх до цього запиту послуги.</span><span class="sxs-lookup"><span data-stu-id="d780c-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="d780c-114">Додаткові ресурси:</span><span class="sxs-lookup"><span data-stu-id="d780c-114">Additional resources:</span></span>

- [<span data-ttu-id="d780c-115">Настроювання Мітки для візуального розмітки для захисту інформації в Azure</span><span class="sxs-lookup"><span data-stu-id="d780c-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="d780c-116">Огляд документації з захисту інформації Azure</span><span class="sxs-lookup"><span data-stu-id="d780c-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="d780c-117">Використання міток чутливості у програмах Office</span><span class="sxs-lookup"><span data-stu-id="d780c-117">Use sensitivity labels in Office apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

