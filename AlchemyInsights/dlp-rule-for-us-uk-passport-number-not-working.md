---
title: ЗВД правило для США/Великобританія номер паспорта не працює
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 3d3b7dc2d9510376bc9eef6ec69b87ad7c681b05
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507319"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="cb0e2-102">Проблеми з ЗВД-US/Великобританія номери паспорта</span><span class="sxs-lookup"><span data-stu-id="cb0e2-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="cb0e2-103">**Важливо**: у ці безпрецедентні часи ми докладаємо всіх зусиль до того, щоб служби SharePoint Online і OneDrive були завжди доступні. Докладні відомості надано у статті [Тимчасові коригування функцій SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="cb0e2-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="cb0e2-104">**ЗВД проблеми з US/Великобританія номери паспорта**</span><span class="sxs-lookup"><span data-stu-id="cb0e2-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="cb0e2-105">У вас виникли проблеми з **запобігання втрати даних (звд)** не працює для вмісту, що містить **номер ПАСПОРТА США/uk** при використанні типу Звд тип інформації в O365?</span><span class="sxs-lookup"><span data-stu-id="cb0e2-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="cb0e2-106">Якщо це так, переконайтеся, що вміст містить потрібну інформацію про те, що в політиці ЗВД шукає, коли його оцінено.</span><span class="sxs-lookup"><span data-stu-id="cb0e2-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="cb0e2-107">Наприклад, для **американського/Великобританії номер паспорта** політики, налаштовані з довірчий рівень 75%, нижче оцінюються і має бути виявлено правило, щоб ініціювати</span><span class="sxs-lookup"><span data-stu-id="cb0e2-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="cb0e2-108">**[Форматі:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Дев'ять цифр</span><span class="sxs-lookup"><span data-stu-id="cb0e2-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nine digits</span></span>

- <span data-ttu-id="cb0e2-109">**[Візерунок:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Дев'ять цифр поспіль</span><span class="sxs-lookup"><span data-stu-id="cb0e2-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="cb0e2-110">**[Контрольна сума:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ні, немає контрольної суми</span><span class="sxs-lookup"><span data-stu-id="cb0e2-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="cb0e2-111">**[Визначення:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** ЗВД політика 75% впевнений, що він виявлений цей тип конфіденційної інформації, якщо в безпосередній близькості від 300 символів:</span><span class="sxs-lookup"><span data-stu-id="cb0e2-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="cb0e2-112">Функція Func_usa_uk_passport знаходить вміст, який відповідає шаблону.</span><span class="sxs-lookup"><span data-stu-id="cb0e2-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="cb0e2-113">Знайдено ключове слово з Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="cb0e2-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="cb0e2-114">Наприклад, наступний зразок буде ініціювати для **США/Великобританія паспорт номер** політики: американський паспорт номер 123456789</span><span class="sxs-lookup"><span data-stu-id="cb0e2-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="cb0e2-115">Для отримання додаткової інформації про те, що потрібно для США/Великобританія номер паспорта, який буде виявлений для вашого контенту, див в наступному розділі в цій статті: [які типи конфіденційної інформації Шукайте нас/номер ПАСПОРТА Великобританії](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="cb0e2-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span></span>
  
<span data-ttu-id="cb0e2-116">Використовуючи інший вбудований тип конфіденційної інформації, зверніться до такої статті, щоб отримати відомості про те, що потрібно для інших типів: [які типи конфіденційних даних шукають](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="cb0e2-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  