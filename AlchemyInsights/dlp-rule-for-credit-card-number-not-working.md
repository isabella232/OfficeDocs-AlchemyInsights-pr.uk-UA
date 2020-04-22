---
title: ЗВД правило для номера кредитної картки не працює
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 80ff41b3e746f95278ccbf0df19eebb61f7f9ee0
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704222"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="39c3e-102">ЗВД питання з номерами кредитних карток</span><span class="sxs-lookup"><span data-stu-id="39c3e-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="39c3e-103">**Важливо**: у ці безпрецедентні часи ми докладаємо всіх зусиль до того, щоб служби SharePoint Online і OneDrive були завжди доступні. Докладні відомості надано у статті [Тимчасові коригування функцій SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="39c3e-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="39c3e-104">**ЗВД питання з номерами кредитних карток**</span><span class="sxs-lookup"><span data-stu-id="39c3e-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="39c3e-105">У вас виникли проблеми з **запобігання втрати даних (звд)** , не працює для вмісту, який містить **номер кредитної картки** під час використання тип інформації з конфіденційною звд в O365?</span><span class="sxs-lookup"><span data-stu-id="39c3e-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="39c3e-106">Якщо так, переконайтеся, що вміст містить потрібну інформацію, щоб ініціювати політику ЗВД під час його обчислення.</span><span class="sxs-lookup"><span data-stu-id="39c3e-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="39c3e-107">Наприклад, для **політики кредитної картки** , настроєної на довірчий рівень 85%, оцінюються і мають бути виявлені правила тригер:</span><span class="sxs-lookup"><span data-stu-id="39c3e-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="39c3e-108">**[Формат:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 цифр, які можуть бути відформатовані або неформатований (ddddddddddddddddddddd) і повинні пройти тест Luhn.</span><span class="sxs-lookup"><span data-stu-id="39c3e-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="39c3e-109">**[Візерунок:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Дуже складний і надійний шаблон, який виявляє карти з усіх основних брендів у всьому світі, включаючи Visa, MasterCard, Discover Card, JCB, American Express, подарункові картки, і закусочної карти.</span><span class="sxs-lookup"><span data-stu-id="39c3e-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="39c3e-110">**[Контрольна сума:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Так, контрольна сума Luhn</span><span class="sxs-lookup"><span data-stu-id="39c3e-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="39c3e-111">**[Визначення:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** ЗВД політика 85% впевнений, що він виявлений цей тип конфіденційної інформації, якщо в безпосередній близькості від 300 символів:</span><span class="sxs-lookup"><span data-stu-id="39c3e-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="39c3e-112">Функція Func_credit_card знаходить вміст, який відповідає шаблону.</span><span class="sxs-lookup"><span data-stu-id="39c3e-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="39c3e-113">Одна з таких дій істинна:</span><span class="sxs-lookup"><span data-stu-id="39c3e-113">One of the following is true:</span></span>

  - <span data-ttu-id="39c3e-114">Знайдено ключове слово з Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="39c3e-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="39c3e-115">Знайдено ключове слово з Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="39c3e-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="39c3e-116">Функція Func_expiration_date знаходить дату в потрібному форматі дати.</span><span class="sxs-lookup"><span data-stu-id="39c3e-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="39c3e-117">Контрольна сума переходить</span><span class="sxs-lookup"><span data-stu-id="39c3e-117">The checksum passes</span></span>

    <span data-ttu-id="39c3e-118">Наприклад, наведений нижче зразок буде викликати на політику ЗВД кредитна картка номер:</span><span class="sxs-lookup"><span data-stu-id="39c3e-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="39c3e-119">Віза: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="39c3e-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="39c3e-120">Термін дії: 2/2009</span><span class="sxs-lookup"><span data-stu-id="39c3e-120">Expires: 2/2009</span></span>

<span data-ttu-id="39c3e-121">Для отримання додаткової інформації про те, що потрібно для того, щоб **номер кредитної картки** був виявлений для вашого вмісту, див у цьому розділі в цій статті: [які типи конфіденційної інформації Шукайте кредитну картку #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="39c3e-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="39c3e-122">Використовуючи інший вбудований тип конфіденційної інформації, зверніться до такої статті, щоб отримати відомості про те, що потрібно для інших типів: [які типи конфіденційних даних шукають](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="39c3e-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  