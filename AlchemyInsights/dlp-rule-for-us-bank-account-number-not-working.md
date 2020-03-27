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
ms.openlocfilehash: bb7d8ca91af73fa4ebed5992ec848128beb18830
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977183"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="2a71d-102">ЗВД питання з номерами банківських рахунків США</span><span class="sxs-lookup"><span data-stu-id="2a71d-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="2a71d-103">**Важливо**: у ці безпрецедентні часи Ми вживаємо заходів, щоб гарантувати, що служби SharePoint Online та OneDrive залишаються доступними – будь ласка, відвідайте [тимчасові функції SharePoint Online](https://aka.ms/ODSPAdjustments) для отримання додаткових відомостей.</span><span class="sxs-lookup"><span data-stu-id="2a71d-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="2a71d-104">**ЗВД питання з номерами банківських рахунків США**</span><span class="sxs-lookup"><span data-stu-id="2a71d-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="2a71d-105">У вас виникли проблеми з **запобігання втрати даних (звд)** , не працює для вмісту, який містить **номер банківського рахунку в США** під час використання тип Звд конфіденційної інформації в O365?</span><span class="sxs-lookup"><span data-stu-id="2a71d-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="2a71d-106">Якщо це так, переконайтеся, що вміст містить потрібну інформацію про те, що в політиці ЗВД шукає, коли його оцінено.</span><span class="sxs-lookup"><span data-stu-id="2a71d-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="2a71d-107">Наприклад, для **американського банківського рахунку** політику, настроєну довірчий рівень 85%, оцінюються і має бути виявлено для запуску правила:</span><span class="sxs-lookup"><span data-stu-id="2a71d-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="2a71d-108">**[Формат:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 цифр</span><span class="sxs-lookup"><span data-stu-id="2a71d-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="2a71d-109">**[Візерунок:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 послідовних цифр.</span><span class="sxs-lookup"><span data-stu-id="2a71d-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="2a71d-110">**[Контрольна сума:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ні, немає контрольної суми</span><span class="sxs-lookup"><span data-stu-id="2a71d-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="2a71d-111">**[Визначення:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** ЗВД політика 75% впевнений, що він виявлений цей тип конфіденційної інформації, якщо в безпосередній близькості від 300 символів:</span><span class="sxs-lookup"><span data-stu-id="2a71d-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="2a71d-112">Регулярний вираз Regex_usa_bank_account_number знаходить вміст, який відповідає шаблону</span><span class="sxs-lookup"><span data-stu-id="2a71d-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="2a71d-113">Знайдено ключове слово з Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="2a71d-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="2a71d-114">Наприклад, наведений нижче зразок може викликати для **американського банківського рахунку** політики: розрахунковий рахунок 78344011</span><span class="sxs-lookup"><span data-stu-id="2a71d-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="2a71d-115">Для отримання додаткової інформації про те, що потрібно для того, щоб **номер банківського рахунку США** був виявлений для вашого вмісту, перегляньте наступний розділ у цій статті: [які типи конфіденційної інформації Шукайте номер банківського рахунку США](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="2a71d-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="2a71d-116">Використовуючи інший вбудований тип конфіденційної інформації, зверніться до такої статті, щоб отримати відомості про те, що потрібно для інших типів: [які типи конфіденційних даних шукають](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="2a71d-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  