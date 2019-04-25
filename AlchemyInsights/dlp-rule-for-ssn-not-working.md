---
title: DLP правило для SSN не працює
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: d2d21fb5546d36990d69b76e3ceb72ce2edf3d80
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404438"
---
<span data-ttu-id="a35b3-102">Вам мають проблеми з **Запобігання втрати даних (DLP)** не працює для вмісту, який містить **Номер соціального страхування Соціального страхування** при використанні конфіденційної інформації типу у службі Office 365</span><span class="sxs-lookup"><span data-stu-id="a35b3-102">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="a35b3-103">Якщо це так, переконайтеся, що ваш зміст містить необхідну інформацію за те, що політика DLP дивлячись.</span><span class="sxs-lookup"><span data-stu-id="a35b3-103">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="a35b3-104">Наприклад, для SSN політику настроєно з рівня довіри до 85%, такі оцінюються і повинні бути виявлені правило викликати:</span><span class="sxs-lookup"><span data-stu-id="a35b3-104">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="a35b3-105">**[Формат:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 цифр, які можуть бути в форматований або неформатований візерунком</span><span class="sxs-lookup"><span data-stu-id="a35b3-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span> 
    
- <span data-ttu-id="a35b3-106">**[Моделі:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Чотири функції шукати SSNs в чотирьох різних моделей:</span><span class="sxs-lookup"><span data-stu-id="a35b3-106">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span> 
    
  - <span data-ttu-id="a35b3-107">Func_ssn знаходить SSNs з попередньо-2011 сильний форматування, відформатовані з тире або пробілів (ddd dd dddd OR ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="a35b3-107">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>
    
  - <span data-ttu-id="a35b3-108">Func_unformatted_ssn знаходить SSNs з попередньо-2011 сильний форматування, які не було відформатовано як дев'ять послідовні цифри (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="a35b3-108">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>
    
  - <span data-ttu-id="a35b3-109">Func_randomized_formatted_ssn знаходить пост-2011 SSNs, які відформатовано з тире або пробілів (ddd dd dddd OR ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="a35b3-109">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>
    
  - <span data-ttu-id="a35b3-110">Func_randomized_unformatted_ssn знаходить пост-2011 SSNs, які є неформатований як дев'ять послідовні цифри (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="a35b3-110">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>
    
- <span data-ttu-id="a35b3-111">**[Контрольна сума:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Ні, немає не контрольної суми</span><span class="sxs-lookup"><span data-stu-id="a35b3-111">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="a35b3-112">**[Визначення:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP політика – 85% впевнені, що вона виявила цей тип конфіденційну інформацію if, в безпосередній близькості від 300 символів:</span><span class="sxs-lookup"><span data-stu-id="a35b3-112">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="a35b3-113">[Функція Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) знаходить вміст, який відповідає візерунку.</span><span class="sxs-lookup"><span data-stu-id="a35b3-113">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span> 
    
  - <span data-ttu-id="a35b3-114">Ключове слово з [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) знайшов.</span><span class="sxs-lookup"><span data-stu-id="a35b3-114">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="a35b3-115">Прикладами ключові слова: *соціальне забезпечення, соціальне забезпечення #, Soc сек, SSN* .</span><span class="sxs-lookup"><span data-stu-id="a35b3-115">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="a35b3-116">Наприклад, у наведеному прикладі ініціює DLP SSN політики: **SSN: 36-489-8350**</span><span class="sxs-lookup"><span data-stu-id="a35b3-116">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
    
<span data-ttu-id="a35b3-117">Більш докладну інформацію про те, що вимагається для SSNs бути виявлені за ваш контент у розділі нижче в цій статті: [Те, що конфіденційних відомостей, надання яких шукати SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="a35b3-117">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="a35b3-118">За допомогою різних вбудований конфіденційної інформації типу, див. відомості про те, що вимагається для інших типів: [що конфіденційних відомостей, надання яких шукати](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="a35b3-118">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

