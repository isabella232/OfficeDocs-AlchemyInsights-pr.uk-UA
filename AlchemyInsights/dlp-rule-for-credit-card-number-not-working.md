---
title: ЗВД правило для номера кредитної картки не працює
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932464"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="71a94-102">ЗВД питання з номерами кредитних карток</span><span class="sxs-lookup"><span data-stu-id="71a94-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="71a94-103">**Важливо**: багато SharePoint Online і OneDrive клієнтів, запустіть бізнес-критичних програм від служби, які працюють у фоновому режимі.</span><span class="sxs-lookup"><span data-stu-id="71a94-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="71a94-104">До них відносяться міграція вмісту, запобігання втрати даних (ЗВД) і рішення для резервного копіювання.</span><span class="sxs-lookup"><span data-stu-id="71a94-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="71a94-105">У ці безпрецедентні часи Ми вживаємо заходів, щоб гарантувати, що служби SharePoint Online та OneDrive залишаються дуже доступними та надійними для користувачів, які залежать від служби, ніж будь-коли в віддалених сценаріях роботи.</span><span class="sxs-lookup"><span data-stu-id="71a94-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="71a94-106">На підтримку цієї мети, ми реалізували жорсткі обмеження регулювання на фонових програм (міграція, ЗВД і резервне копіювання рішень) в будні дні вдень.</span><span class="sxs-lookup"><span data-stu-id="71a94-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="71a94-107">Ви повинні очікувати, що ці програми будуть досягати дуже обмежену пропускну здатність в ці часи.</span><span class="sxs-lookup"><span data-stu-id="71a94-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="71a94-108">Однак під час вечірніх та вихідних годин для регіону служба буде готова обробляти значно більший обсяг запитів від фонових програм.</span><span class="sxs-lookup"><span data-stu-id="71a94-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="71a94-109">**ЗВД питання з номерами кредитних карток**</span><span class="sxs-lookup"><span data-stu-id="71a94-109">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="71a94-110">У вас виникли проблеми з **запобігання втрати даних (звд)** , не працює для вмісту, який містить **номер кредитної картки** під час використання тип інформації з конфіденційною звд в O365?</span><span class="sxs-lookup"><span data-stu-id="71a94-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="71a94-111">Якщо так, переконайтеся, що вміст містить потрібну інформацію, щоб ініціювати політику ЗВД під час його обчислення.</span><span class="sxs-lookup"><span data-stu-id="71a94-111">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="71a94-112">Наприклад, для **політики кредитної картки** , настроєної на довірчий рівень 85%, оцінюються і мають бути виявлені правила тригер:</span><span class="sxs-lookup"><span data-stu-id="71a94-112">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="71a94-113">**[Формат:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 цифр, які можуть бути відформатовані або неформатований (ddddddddddddddddddddd) і повинні пройти тест Luhn.</span><span class="sxs-lookup"><span data-stu-id="71a94-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="71a94-114">**[Візерунок:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Дуже складний і надійний шаблон, який виявляє карти з усіх основних брендів у всьому світі, включаючи Visa, MasterCard, Discover Card, JCB, American Express, подарункові картки, і закусочної карти.</span><span class="sxs-lookup"><span data-stu-id="71a94-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="71a94-115">**[Контрольна сума:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Так, контрольна сума Luhn</span><span class="sxs-lookup"><span data-stu-id="71a94-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="71a94-116">**[Визначення:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** ЗВД політика 85% впевнений, що він виявлений цей тип конфіденційної інформації, якщо в безпосередній близькості від 300 символів:</span><span class="sxs-lookup"><span data-stu-id="71a94-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="71a94-117">Функція Func_credit_card знаходить вміст, який відповідає шаблону.</span><span class="sxs-lookup"><span data-stu-id="71a94-117">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="71a94-118">Одна з таких дій істинна:</span><span class="sxs-lookup"><span data-stu-id="71a94-118">One of the following is true:</span></span>

  - <span data-ttu-id="71a94-119">Знайдено ключове слово з Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="71a94-119">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="71a94-120">Знайдено ключове слово з Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="71a94-120">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="71a94-121">Функція Func_expiration_date знаходить дату в потрібному форматі дати.</span><span class="sxs-lookup"><span data-stu-id="71a94-121">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="71a94-122">Контрольна сума переходить</span><span class="sxs-lookup"><span data-stu-id="71a94-122">The checksum passes</span></span>

    <span data-ttu-id="71a94-123">Наприклад, наведений нижче зразок буде викликати на політику ЗВД кредитна картка номер:</span><span class="sxs-lookup"><span data-stu-id="71a94-123">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="71a94-124">Віза: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="71a94-124">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="71a94-125">Термін дії: 2/2009</span><span class="sxs-lookup"><span data-stu-id="71a94-125">Expires: 2/2009</span></span>

<span data-ttu-id="71a94-126">Для отримання додаткової інформації про те, що потрібно для того, щоб **номер кредитної картки** був виявлений для вашого вмісту, див у цьому розділі в цій статті: [які типи конфіденційної інформації Шукайте кредитну картку #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="71a94-126">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="71a94-127">Використовуючи інший вбудований тип конфіденційної інформації, зверніться до такої статті, щоб отримати відомості про те, що потрібно для інших типів: [які типи конфіденційних даних шукають](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="71a94-127">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  