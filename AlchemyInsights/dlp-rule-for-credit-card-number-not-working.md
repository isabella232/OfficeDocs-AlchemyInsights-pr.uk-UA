---
title: Правило DLP для номера кредитної картки не працює
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679462"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="01a5b-102">Проблеми з DLP з номерами кредитних карток</span><span class="sxs-lookup"><span data-stu-id="01a5b-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="01a5b-103">**Важливо**: у ці безпрецедентні часи ми докладаємо всіх зусиль до того, щоб служби SharePoint Online і OneDrive були завжди доступні. Докладні відомості надано у статті [Тимчасові коригування функцій SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="01a5b-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="01a5b-104">**Проблеми з DLP з номерами кредитних карток**</span><span class="sxs-lookup"><span data-stu-id="01a5b-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="01a5b-105">У вас виникли проблеми з **запобіганням втрати даних (DLP)** , які не працюють для вмісту, що містить **номер кредитної картки** , якщо використовується тип конфіденційної інформації DLP у O365?</span><span class="sxs-lookup"><span data-stu-id="01a5b-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="01a5b-106">Якщо це так, переконайтеся, що вміст містить необхідну інформацію, щоб ініціювати політику DLP, коли її оцінено.</span><span class="sxs-lookup"><span data-stu-id="01a5b-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="01a5b-107">Наприклад, для **політики кредитної картки** , настроєної на рівень впевненості в 85%, наведені нижче оцінки та мають виявлятися для показу правила.</span><span class="sxs-lookup"><span data-stu-id="01a5b-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="01a5b-108">**[Формат:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 цифр, які можуть бути відформатовані або неформатовані (dddddddddddddddd) і повинні пройти тест Luhn.</span><span class="sxs-lookup"><span data-stu-id="01a5b-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="01a5b-109">**[Візерунок:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Дуже складний і надійний візерунок, який виявляє картки з усіх основних брендів по всьому світу, зокрема Visa, MasterCard, Discover картки, JCB, American Express, подарункових карток і карток Diner.</span><span class="sxs-lookup"><span data-stu-id="01a5b-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="01a5b-110">**[Контрольна сума:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Так, контрольна сума Luhn</span><span class="sxs-lookup"><span data-stu-id="01a5b-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="01a5b-111">**[Визначення:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Політика DLP – 85% упевнений, що це тип конфіденційної інформації, якщо в безпосередній близькості від 300 символів:</span><span class="sxs-lookup"><span data-stu-id="01a5b-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="01a5b-112">Функція Func_credit_card знаходить вміст, який відповідає шаблону.</span><span class="sxs-lookup"><span data-stu-id="01a5b-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="01a5b-113">Один із наведених нижче варіантів має значення ІСТИНА.</span><span class="sxs-lookup"><span data-stu-id="01a5b-113">One of the following is true:</span></span>

  - <span data-ttu-id="01a5b-114">Виявлено ключове слово з Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="01a5b-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="01a5b-115">Знайдено ключове слово з Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="01a5b-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="01a5b-116">Функція Func_expiration_date знаходить дату в правильному форматі дати.</span><span class="sxs-lookup"><span data-stu-id="01a5b-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="01a5b-117">Контрольна сума проходить</span><span class="sxs-lookup"><span data-stu-id="01a5b-117">The checksum passes</span></span>

    <span data-ttu-id="01a5b-118">Наприклад, наведений нижче зразок буде тригер для політики номера кредитної картки DLP:</span><span class="sxs-lookup"><span data-stu-id="01a5b-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="01a5b-119">Віза: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="01a5b-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="01a5b-120">Термін дії: 2/2009</span><span class="sxs-lookup"><span data-stu-id="01a5b-120">Expires: 2/2009</span></span>

<span data-ttu-id="01a5b-121">Щоб отримати докладні відомості про те, що потрібно знайти для вашого вмісту **номер кредитної картки** , ознайомтеся з такими розділами в цій статті: [що таке важливі типи даних, які шукають кредитну картку #](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="01a5b-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span></span>
  
<span data-ttu-id="01a5b-122">Використовуючи інший вбудований тип конфіденційної інформації, ознайомтеся з наведена нижче стаття для отримання відомостей про те, що необхідно для інших типів: [які типи важливих відомостей відображаються](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="01a5b-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  