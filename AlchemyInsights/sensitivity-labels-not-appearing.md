---
title: Не відображаються позначки чутливості
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 72dc88a55b55954f34c95fa5b5038f472261c5bb
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758538"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="30566-102">Не відображаються позначки чутливості</span><span class="sxs-lookup"><span data-stu-id="30566-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="30566-103">За допомогою міток чутливості можна класифікувати та захищати вміст делікатного характеру.</span><span class="sxs-lookup"><span data-stu-id="30566-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="30566-104">Вони можуть бути створені в Microsoft 365 центр відповідності, Microsoft 365 Центр безпеки, або Microsoft 365 безпеки & центр відповідності класифікації > чутливість етикетки.</span><span class="sxs-lookup"><span data-stu-id="30566-104">They can be created in the Microsoft 365 compliance center, Microsoft 365 security center, or Microsoft 365 security & Compliance Center under Classification > Sensitivity labels.</span></span> <span data-ttu-id="30566-105">Щоб дізнатися більше про цю функцію, перегляньте [Огляд міток чутливості](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).</span><span class="sxs-lookup"><span data-stu-id="30566-105">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).</span></span>

<span data-ttu-id="30566-106">Якщо ви налаштували Мітки чутливості, але вони не відображаються в застосунках Office, перевірте наступне:</span><span class="sxs-lookup"><span data-stu-id="30566-106">If you configured your sensitivity labels but they aren't appearing in the Office apps, check the following:</span></span>

- <span data-ttu-id="30566-107">Переконайтеся, що підпис чутливості [Опубліковано](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) користувачам і групам, які ви хочете.</span><span class="sxs-lookup"><span data-stu-id="30566-107">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="30566-108">Переконайтеся, що користувач використовує програму, яка [підтримує Мітки чутливості-див.](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable)</span><span class="sxs-lookup"><span data-stu-id="30566-108">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span></span>

- <span data-ttu-id="30566-109">Якщо ви [переміщуєте підписи захисту інформації до Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), зверніть увагу на міркування, перелічені [тут](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span><span class="sxs-lookup"><span data-stu-id="30566-109">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="30566-110">Підтримка запобігання втраті даних (ЗВД): наразі лише підписи збереження можуть використовуватися як умова в політиці ЗВД.</span><span class="sxs-lookup"><span data-stu-id="30566-110">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="30566-111">Підтримка Мітки чутливості у ЗВД політика ще недоступна, але ми працюємо над цим.</span><span class="sxs-lookup"><span data-stu-id="30566-111">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

- <span data-ttu-id="30566-112">Коли шифрування ввімкнено для Мітки чутливості, ви можете вибрати один із таких:</span><span class="sxs-lookup"><span data-stu-id="30566-112">When encryption is enabled on a sensitivity label, you can choose either to:</span></span>
    - <span data-ttu-id="30566-113">Призначити дозволи зараз</span><span class="sxs-lookup"><span data-stu-id="30566-113">Assign permissions now</span></span>
    - <span data-ttu-id="30566-114">Дозволити користувачам призначати дозволи</span><span class="sxs-lookup"><span data-stu-id="30566-114">Let users assign permissions</span></span>


<span data-ttu-id="30566-115">Щоб отримати додаткові відомості про можливі проблеми, перегляньте [відомі проблеми з мітками чутливості](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span><span class="sxs-lookup"><span data-stu-id="30566-115">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span></span>