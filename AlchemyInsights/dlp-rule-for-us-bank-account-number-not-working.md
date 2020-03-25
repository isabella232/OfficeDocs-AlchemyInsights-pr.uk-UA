---
title: "\"ЗВД\" правило для номера банківського рахунку США не працює"
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 0b5c1fb175275028c56e47080708520fe115fb38
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932571"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="85e2e-102">ЗВД питання з номерами банківських рахунків США</span><span class="sxs-lookup"><span data-stu-id="85e2e-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="85e2e-103">**Важливо**: багато SharePoint Online і OneDrive клієнтів, запустіть бізнес-критичних програм від служби, які працюють у фоновому режимі.</span><span class="sxs-lookup"><span data-stu-id="85e2e-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="85e2e-104">До них відносяться міграція вмісту, запобігання втрати даних (ЗВД) і рішення для резервного копіювання.</span><span class="sxs-lookup"><span data-stu-id="85e2e-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="85e2e-105">У ці безпрецедентні часи Ми вживаємо заходів, щоб гарантувати, що служби SharePoint Online та OneDrive залишаються дуже доступними та надійними для користувачів, які залежать від служби, ніж будь-коли в віддалених сценаріях роботи.</span><span class="sxs-lookup"><span data-stu-id="85e2e-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="85e2e-106">На підтримку цієї мети, ми реалізували жорсткі обмеження регулювання на фонових програм (міграція, ЗВД і резервне копіювання рішень) в будні дні вдень.</span><span class="sxs-lookup"><span data-stu-id="85e2e-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="85e2e-107">Ви повинні очікувати, що ці програми будуть досягати дуже обмежену пропускну здатність в ці часи.</span><span class="sxs-lookup"><span data-stu-id="85e2e-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="85e2e-108">Однак під час вечірніх та вихідних годин для регіону служба буде готова обробляти значно більший обсяг запитів від фонових програм.</span><span class="sxs-lookup"><span data-stu-id="85e2e-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="85e2e-109">**ЗВД питання з номерами банківських рахунків США**</span><span class="sxs-lookup"><span data-stu-id="85e2e-109">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="85e2e-110">У вас виникли проблеми з **запобігання втрати даних (звд)** , не працює для вмісту, який містить **номер банківського рахунку в США** під час використання тип Звд конфіденційної інформації в O365?</span><span class="sxs-lookup"><span data-stu-id="85e2e-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="85e2e-111">Якщо це так, переконайтеся, що вміст містить потрібну інформацію про те, що в політиці ЗВД шукає, коли його оцінено.</span><span class="sxs-lookup"><span data-stu-id="85e2e-111">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="85e2e-112">Наприклад, для **американського банківського рахунку** політику, настроєну довірчий рівень 85%, оцінюються і має бути виявлено для запуску правила:</span><span class="sxs-lookup"><span data-stu-id="85e2e-112">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="85e2e-113">**[Формат:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 цифр</span><span class="sxs-lookup"><span data-stu-id="85e2e-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="85e2e-114">**[Візерунок:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 послідовних цифр.</span><span class="sxs-lookup"><span data-stu-id="85e2e-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="85e2e-115">**[Контрольна сума:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ні, немає контрольної суми</span><span class="sxs-lookup"><span data-stu-id="85e2e-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="85e2e-116">**[Визначення:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** ЗВД політика 75% впевнений, що він виявлений цей тип конфіденційної інформації, якщо в безпосередній близькості від 300 символів:</span><span class="sxs-lookup"><span data-stu-id="85e2e-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="85e2e-117">Регулярний вираз Regex_usa_bank_account_number знаходить вміст, який відповідає шаблону</span><span class="sxs-lookup"><span data-stu-id="85e2e-117">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="85e2e-118">Знайдено ключове слово з Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="85e2e-118">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="85e2e-119">Наприклад, наведений нижче зразок може викликати для **американського банківського рахунку** політики: розрахунковий рахунок 78344011</span><span class="sxs-lookup"><span data-stu-id="85e2e-119">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="85e2e-120">Для отримання додаткової інформації про те, що потрібно для того, щоб **номер банківського рахунку США** був виявлений для вашого вмісту, перегляньте наступний розділ у цій статті: [які типи конфіденційної інформації Шукайте номер банківського рахунку США](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="85e2e-120">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="85e2e-121">Використовуючи інший вбудований тип конфіденційної інформації, зверніться до такої статті, щоб отримати відомості про те, що потрібно для інших типів: [які типи конфіденційних даних шукають](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="85e2e-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  