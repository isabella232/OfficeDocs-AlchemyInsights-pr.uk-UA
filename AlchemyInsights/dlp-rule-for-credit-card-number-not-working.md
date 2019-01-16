---
title: DLP правило для номер кредитної картки, не працює
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: a56f32b54e6cb32fa044d26d08868bac8c368de5
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/15/2019
ms.locfileid: "28318983"
---
<span data-ttu-id="ed2b9-p101">Виникли проблеми із **Запобігання втрати даних (DLP)** не працює для вмісту, який містить **Номер кредитної картки** , при використанні DLP конфіденційної інформації типу в O365? Якщо це так, переконайтеся, що ваш зміст містить необхідну інформацію, щоб викликати в DLP політики, коли його оцінка. Наприклад, для **кредитних карт політики** з рівня довіри до 85%, такі оцінюються і повинні бути виявлені правило викликати:</span><span class="sxs-lookup"><span data-stu-id="ed2b9-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated. For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="ed2b9-105">**[Формат:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 цифр, яке можна форматувати або неформатований (dddddddddddddddd) і має пройти тест на Luhn.</span><span class="sxs-lookup"><span data-stu-id="ed2b9-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span> 
    
- <span data-ttu-id="ed2b9-106">**[Моделі:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Дуже складний і надійний зразок, який виявляє карт від всі основні бренди по всьому світу, включаючи Visa, Mastercard, Discover Card, JCB, American Express, подарункових карток і карток diner.</span><span class="sxs-lookup"><span data-stu-id="ed2b9-106">**[Pattern:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span> 
    
- <span data-ttu-id="ed2b9-107">**[Контрольна сума:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Так, Luhn контрольної суми</span><span class="sxs-lookup"><span data-stu-id="ed2b9-107">**[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span> 
    
- <span data-ttu-id="ed2b9-108">**[Визначення:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP політика – 85% впевнені, що вона виявила цей тип конфіденційну інформацію if, в безпосередній близькості від 300 символів:</span><span class="sxs-lookup"><span data-stu-id="ed2b9-108">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="ed2b9-109">Функція Func_credit_card знаходить вміст, який відповідає візерунку.</span><span class="sxs-lookup"><span data-stu-id="ed2b9-109">The function Func_credit_card finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="ed2b9-110">Одна з таких вірна:</span><span class="sxs-lookup"><span data-stu-id="ed2b9-110">One of the following is true:</span></span> 
    
  - <span data-ttu-id="ed2b9-111">Ключове слово з Keyword_cc_verification знайшов.</span><span class="sxs-lookup"><span data-stu-id="ed2b9-111">A keyword from Keyword_cc_verification is found.</span></span>
    
  - <span data-ttu-id="ed2b9-112">Ключове слово з Keyword_cc_name знайдені</span><span class="sxs-lookup"><span data-stu-id="ed2b9-112">A keyword from Keyword_cc_name is found</span></span>
    
  - <span data-ttu-id="ed2b9-113">Функція Func_expiration_date знаходить дату у форматі дати правильний.</span><span class="sxs-lookup"><span data-stu-id="ed2b9-113">The function Func_expiration_date finds a date in the right date format.</span></span>
    
  - <span data-ttu-id="ed2b9-114">Контрольна сума проходить</span><span class="sxs-lookup"><span data-stu-id="ed2b9-114">The checksum passes</span></span>
    
    <span data-ttu-id="ed2b9-115">Наприклад, у наведеному прикладі ініціює DLP кредитної картки номер політики:</span><span class="sxs-lookup"><span data-stu-id="ed2b9-115">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>
    
  - <span data-ttu-id="ed2b9-116">Віза: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="ed2b9-116">Visa: 4485 3647 3952 7352</span></span> 
    
  - <span data-ttu-id="ed2b9-117">Термін дії: 2/2009</span><span class="sxs-lookup"><span data-stu-id="ed2b9-117">Expires: 2/2009</span></span>
    
<span data-ttu-id="ed2b9-118">Більш докладну інформацію про те, що вимагається для **Номер кредитної картки** , щоб бути виявлені за ваш контент у розділі нижче в цій статті: [Те, що чутливої інформації типи шукати кредитної картки #](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="ed2b9-118">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="ed2b9-119">За допомогою різних вбудований конфіденційної інформації типу, див. відомості про те, що вимагається для інших типів: [що конфіденційних відомостей, надання яких шукати](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="ed2b9-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

