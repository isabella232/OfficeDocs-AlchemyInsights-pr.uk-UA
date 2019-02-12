---
title: DLP правило для нас номер банківського рахунку не працює
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 9ebfa6bc09cef9ab7c30bddb4fcb8b6be3ab55a5
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29916437"
---
<span data-ttu-id="dfc0d-p101">Виникли проблеми із **Запобігання втрати даних (DLP)** не працює для вмісту, який містить **Номер банківського рахунку США** при використанні DLP конфіденційної інформації типу в O365? Якщо це так, переконайтеся, що ваш зміст містить необхідну інформацію для що DLP політики шукає коли його оцінка.</span><span class="sxs-lookup"><span data-stu-id="dfc0d-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="dfc0d-104">Наприклад, для політики **США номер банківського рахунку** з рівня довіри до 85%, такі оцінюються і повинні бути виявлені правило викликати:</span><span class="sxs-lookup"><span data-stu-id="dfc0d-104">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="dfc0d-105">**[Формат:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 цифр</span><span class="sxs-lookup"><span data-stu-id="dfc0d-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span> 
    
- <span data-ttu-id="dfc0d-106">**[Моделі:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 послідовних цифр.</span><span class="sxs-lookup"><span data-stu-id="dfc0d-106">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span> 
    
- <span data-ttu-id="dfc0d-107">**[Контрольна сума:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ні, немає не контрольної суми</span><span class="sxs-lookup"><span data-stu-id="dfc0d-107">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="dfc0d-108">**[Визначення:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** DLP політика – 75% впевнені, що вона виявила цей тип конфіденційну інформацію if, в безпосередній близькості від 300 символів:</span><span class="sxs-lookup"><span data-stu-id="dfc0d-108">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="dfc0d-109">Регулярний вираз Regex_usa_bank_account_number знаходить вміст, який відповідає візерунку</span><span class="sxs-lookup"><span data-stu-id="dfc0d-109">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>
    
  - <span data-ttu-id="dfc0d-110">Ключове слово з Keyword_usa_Bank_Account знайшов.</span><span class="sxs-lookup"><span data-stu-id="dfc0d-110">A keyword from Keyword_usa_Bank_Account is found.</span></span>
    
    <span data-ttu-id="dfc0d-111">Наприклад, у наведеному прикладі ініціює політики **США номер банківського рахунку** : розрахунковий рахунок 78344011</span><span class="sxs-lookup"><span data-stu-id="dfc0d-111">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span> 
    
<span data-ttu-id="dfc0d-112">Більш докладну інформацію про те, що вимагається для **США номер банківського рахунку** , щоб бути виявлені за ваш контент у розділі нижче в цій статті: [Те, що чутливої інформації типи шукати номер банківського рахунку в США](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="dfc0d-112">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="dfc0d-113">За допомогою різних вбудований конфіденційної інформації типу, див. відомості про те, що вимагається для інших типів: [що конфіденційних відомостей, надання яких шукати](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="dfc0d-113">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

