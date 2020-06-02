---
title: "\"ЗВД\" правило для номера банківського рахунку США не працює"
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: b032a7c80e8b387114aeda95c4f6af7e57225517
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507355"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="8db34-102">ЗВД питання з номерами банківських рахунків США</span><span class="sxs-lookup"><span data-stu-id="8db34-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="8db34-103">**Важливо**: у ці безпрецедентні часи ми докладаємо всіх зусиль до того, щоб служби SharePoint Online і OneDrive були завжди доступні. Докладні відомості надано у статті [Тимчасові коригування функцій SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="8db34-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="8db34-104">**ЗВД питання з номерами банківських рахунків США**</span><span class="sxs-lookup"><span data-stu-id="8db34-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="8db34-105">У вас виникли проблеми з **запобігання втрати даних (звд)** , не працює для вмісту, який містить **номер банківського рахунку в США** під час використання тип Звд конфіденційної інформації в O365?</span><span class="sxs-lookup"><span data-stu-id="8db34-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="8db34-106">Якщо це так, переконайтеся, що вміст містить потрібну інформацію про те, що в політиці ЗВД шукає, коли його оцінено.</span><span class="sxs-lookup"><span data-stu-id="8db34-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="8db34-107">Наприклад, для **американського банківського рахунку** політику, настроєну довірчий рівень 85%, оцінюються і має бути виявлено для запуску правила:</span><span class="sxs-lookup"><span data-stu-id="8db34-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="8db34-108">**[Формат:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 цифр</span><span class="sxs-lookup"><span data-stu-id="8db34-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="8db34-109">**[Візерунок:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 послідовних цифр.</span><span class="sxs-lookup"><span data-stu-id="8db34-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="8db34-110">**[Контрольна сума:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ні, немає контрольної суми</span><span class="sxs-lookup"><span data-stu-id="8db34-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="8db34-111">**[Визначення:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** ЗВД політика 75% впевнений, що він виявлений цей тип конфіденційної інформації, якщо в безпосередній близькості від 300 символів:</span><span class="sxs-lookup"><span data-stu-id="8db34-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="8db34-112">Регулярний вираз Regex_usa_bank_account_number знаходить вміст, який відповідає шаблону</span><span class="sxs-lookup"><span data-stu-id="8db34-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="8db34-113">Знайдено ключове слово з Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="8db34-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="8db34-114">Наприклад, наведений нижче зразок може викликати для **американського банківського рахунку** політики: розрахунковий рахунок 78344011</span><span class="sxs-lookup"><span data-stu-id="8db34-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="8db34-115">Для отримання додаткової інформації про те, що потрібно для того, щоб **номер банківського рахунку США** був виявлений для вашого вмісту, перегляньте наступний розділ у цій статті: [які типи конфіденційної інформації Шукайте номер банківського рахунку США](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="8db34-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span></span>
  
<span data-ttu-id="8db34-116">Використовуючи інший вбудований тип конфіденційної інформації, зверніться до такої статті, щоб отримати відомості про те, що потрібно для інших типів: [які типи конфіденційних даних шукають](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="8db34-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  