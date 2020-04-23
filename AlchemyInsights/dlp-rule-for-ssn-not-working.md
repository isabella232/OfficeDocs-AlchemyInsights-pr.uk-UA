---
title: ЗВД правило для SSN не працює
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 5af843c2b70b5b2e1aaf82c9f01356546929d840
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43788723"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="fad8e-102">ЗВД питання з номерами соціального страхування</span><span class="sxs-lookup"><span data-stu-id="fad8e-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="fad8e-103">**Важливо**: у ці безпрецедентні часи ми докладаємо всіх зусиль до того, щоб служби SharePoint Online і OneDrive були завжди доступні. Докладні відомості надано у статті [Тимчасові коригування функцій SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="fad8e-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="fad8e-104">**ЗВД проблеми з SSNs**</span><span class="sxs-lookup"><span data-stu-id="fad8e-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="fad8e-105">У вас виникли проблеми з **запобігання втрати даних (звд)** не працює для вмісту, який містить **номер соціального страхування (SSN)** під час використання тип конфіденційної інформації в Microsoft 365?</span><span class="sxs-lookup"><span data-stu-id="fad8e-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="fad8e-106">Якщо це так, переконайтеся, що вміст містить потрібну інформацію про те, що виглядає політика ЗВД.</span><span class="sxs-lookup"><span data-stu-id="fad8e-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="fad8e-107">Наприклад, для політики SSN, настроєної на довірчий рівень 85%, обчислюються такі і повинні бути виявлені правила для запуску:</span><span class="sxs-lookup"><span data-stu-id="fad8e-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="fad8e-108">**[Формат:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 цифр, які можуть бути відформатовані або неформатованим візерунком</span><span class="sxs-lookup"><span data-stu-id="fad8e-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="fad8e-109">**[Візерунок:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Чотири функції Шукайте SSNs в чотирьох різних моделей:</span><span class="sxs-lookup"><span data-stu-id="fad8e-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="fad8e-110">Func_ssn знаходить SSNs з попередньо 2011 стійке форматування, відформатовані дефіси або пробіли (DDD-DD-DDDD або DDD DD DDDD)</span><span class="sxs-lookup"><span data-stu-id="fad8e-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="fad8e-111">Func_unformatted_ssn знаходить SSNs з попередньо 2011 стійке форматування, неформатований як дев'ять цифр (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="fad8e-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="fad8e-112">Func_randomized_formatted_ssn знаходить Post-2011 SSNs, відформатовані за допомогою тире або пробілів (DDD-DD-DDDD або DDD DD DDDD)</span><span class="sxs-lookup"><span data-stu-id="fad8e-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="fad8e-113">Func_randomized_unformatted_ssn знаходить Post-2011 SSNs, які неформатовані як дев'ять цифр (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="fad8e-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="fad8e-114">**[Контрольна сума:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Ні, немає контрольної суми</span><span class="sxs-lookup"><span data-stu-id="fad8e-114">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="fad8e-115">**[Визначення:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** ЗВД політика 85% впевнений, що він виявлений цей тип конфіденційної інформації, якщо в безпосередній близькості від 300 символів:</span><span class="sxs-lookup"><span data-stu-id="fad8e-115">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="fad8e-116">[Функція Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) знаходить вміст, який відповідає шаблону.</span><span class="sxs-lookup"><span data-stu-id="fad8e-116">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="fad8e-117">Знайдено ключове слово з [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) .</span><span class="sxs-lookup"><span data-stu-id="fad8e-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="fad8e-118">Приклади ключових слів включають: *соціальне забезпечення, соціальне забезпечення #, СНС, SSN* .</span><span class="sxs-lookup"><span data-stu-id="fad8e-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="fad8e-119">Наприклад, наведений нижче зразок буде тригер за ЗВД SSN політики: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="fad8e-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="fad8e-120">Для отримання додаткових відомостей про те, що потрібно для виявлення SSNs для вашого вмісту, див у розділі нижче в цій статті: [які типи конфіденційної інформації Шукайте SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="fad8e-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="fad8e-121">Використовуючи інший вбудований тип конфіденційної інформації, зверніться до такої статті, щоб отримати відомості про те, що потрібно для інших типів: [які типи конфіденційних даних шукають](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="fad8e-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  