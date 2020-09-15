---
title: Правило DLP для SSN не працює
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679390"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="dd46d-102">Помилки DLP із номерами соціального страхування</span><span class="sxs-lookup"><span data-stu-id="dd46d-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="dd46d-103">**Важливо**: у ці безпрецедентні часи ми докладаємо всіх зусиль до того, щоб служби SharePoint Online і OneDrive були завжди доступні. Докладні відомості надано у статті [Тимчасові коригування функцій SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="dd46d-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="dd46d-104">**Проблеми з DLP, які містять SSNs**</span><span class="sxs-lookup"><span data-stu-id="dd46d-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="dd46d-105">У вас виникли проблеми з **запобіганням втрати даних (DLP)** , які не працюють для вмісту, що містить **номер соціального страхування (SSN)** під час використання типу конфіденційної інформації в Microsoft 365?</span><span class="sxs-lookup"><span data-stu-id="dd46d-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="dd46d-106">Якщо це так, переконайтеся, що вміст містить потрібні відомості про те, що таке політика DLP шукає.</span><span class="sxs-lookup"><span data-stu-id="dd46d-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="dd46d-107">Наприклад, для політики SSN, настроєного на рівень впевненості в 85%, наведені нижче оцінки та мають виявлятися для запуску правила.</span><span class="sxs-lookup"><span data-stu-id="dd46d-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="dd46d-108">**[Формат:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 цифр, які можуть перебувати в форматованому або неформатований шаблоні</span><span class="sxs-lookup"><span data-stu-id="dd46d-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="dd46d-109">**[Візерунок:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Чотири функції шукають SSNs в чотирьох різних шаблонах:</span><span class="sxs-lookup"><span data-stu-id="dd46d-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="dd46d-110">Func_ssn знаходить SSNs з попередньо 2011 сильним форматуванням, відформатованими з тире або пробілами (DDD-DD-DDDD або DD DD DDDD)</span><span class="sxs-lookup"><span data-stu-id="dd46d-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="dd46d-111">Func_unformatted_ssn знаходить SSNs з попередньо 2011 сильним форматуванням, які не відформатовано як дев'ять послідовних цифр (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="dd46d-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="dd46d-112">Func_randomized_formatted_ssn знаходить пост-2011 SSNs, відформатовані за допомогою тире або пробілів (DDD-DD-DDDD або DD DD DDDD)</span><span class="sxs-lookup"><span data-stu-id="dd46d-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="dd46d-113">Func_randomized_unformatted_ssn знаходить пост-2011 SSNs, які не форматовані як дев'ять послідовних цифр (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="dd46d-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="dd46d-114">**[Контрольна сума:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Ні, немає контрольної суми</span><span class="sxs-lookup"><span data-stu-id="dd46d-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="dd46d-115">**[Визначення:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Політика DLP – 85% упевнений, що це тип конфіденційної інформації, якщо в безпосередній близькості від 300 символів:</span><span class="sxs-lookup"><span data-stu-id="dd46d-115">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="dd46d-116">[Функція Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) знаходить вміст, який відповідає шаблону.</span><span class="sxs-lookup"><span data-stu-id="dd46d-116">The [function Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="dd46d-117">Виявлено ключове слово з [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) .</span><span class="sxs-lookup"><span data-stu-id="dd46d-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found.</span></span> <span data-ttu-id="dd46d-118">Приклади ключових слів:  *Соціальна безпека, соціальне забезпечення #, SOC SEC, SSN*  .</span><span class="sxs-lookup"><span data-stu-id="dd46d-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="dd46d-119">Наприклад, наведений нижче зразок буде тригер для політики DLP SSN: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="dd46d-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="dd46d-120">Щоб отримати докладні відомості про те, що потрібно для SSNs, які потрібно виявити для вашого вмісту, ознайомтеся з цим розділом у цій статті: [які типи конфіденційних даних шукають SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="dd46d-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="dd46d-121">Використовуючи інший вбудований тип конфіденційної інформації, ознайомтеся з наведена нижче стаття для отримання відомостей про те, що необхідно для інших типів: [які типи важливих відомостей відображаються](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="dd46d-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  