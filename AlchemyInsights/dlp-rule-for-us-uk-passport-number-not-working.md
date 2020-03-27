---
title: ЗВД правило для США/Великобританія номер паспорта не працює
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 534e258c31a9a71c618765511487487c53f455b5
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977127"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="d639d-102">Проблеми з ЗВД-US/Великобританія номери паспорта</span><span class="sxs-lookup"><span data-stu-id="d639d-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="d639d-103">**Важливо**: у ці безпрецедентні часи Ми вживаємо заходів, щоб гарантувати, що служби SharePoint Online та OneDrive залишаються доступними – будь ласка, відвідайте [тимчасові функції SharePoint Online](https://aka.ms/ODSPAdjustments) для отримання додаткових відомостей.</span><span class="sxs-lookup"><span data-stu-id="d639d-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="d639d-104">**ЗВД проблеми з US/Великобританія номери паспорта**</span><span class="sxs-lookup"><span data-stu-id="d639d-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="d639d-105">У вас виникли проблеми з **запобігання втрати даних (звд)** не працює для вмісту, що містить **номер ПАСПОРТА США/uk** при використанні типу Звд тип інформації в O365?</span><span class="sxs-lookup"><span data-stu-id="d639d-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="d639d-106">Якщо це так, переконайтеся, що вміст містить потрібну інформацію про те, що в політиці ЗВД шукає, коли його оцінено.</span><span class="sxs-lookup"><span data-stu-id="d639d-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="d639d-107">Наприклад, для **американського/Великобританії номер паспорта** політики, налаштовані з довірчий рівень 75%, нижче оцінюються і має бути виявлено правило, щоб ініціювати</span><span class="sxs-lookup"><span data-stu-id="d639d-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="d639d-108">**[Форматі:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Дев'ять цифр</span><span class="sxs-lookup"><span data-stu-id="d639d-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="d639d-109">**[Візерунок:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Дев'ять цифр поспіль</span><span class="sxs-lookup"><span data-stu-id="d639d-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="d639d-110">**[Контрольна сума:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ні, немає контрольної суми</span><span class="sxs-lookup"><span data-stu-id="d639d-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="d639d-111">**[Визначення:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** ЗВД політика 75% впевнений, що він виявлений цей тип конфіденційної інформації, якщо в безпосередній близькості від 300 символів:</span><span class="sxs-lookup"><span data-stu-id="d639d-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="d639d-112">Функція Func_usa_uk_passport знаходить вміст, який відповідає шаблону.</span><span class="sxs-lookup"><span data-stu-id="d639d-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="d639d-113">Знайдено ключове слово з Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="d639d-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="d639d-114">Наприклад, наступний зразок буде ініціювати для **США/Великобританія паспорт номер** політики: американський паспорт номер 123456789</span><span class="sxs-lookup"><span data-stu-id="d639d-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="d639d-115">Для отримання додаткової інформації про те, що потрібно для США/Великобританія номер паспорта, який буде виявлений для вашого контенту, див в наступному розділі в цій статті: [які типи конфіденційної інформації Шукайте нас/номер ПАСПОРТА Великобританії](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="d639d-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="d639d-116">Використовуючи інший вбудований тип конфіденційної інформації, зверніться до такої статті, щоб отримати відомості про те, що потрібно для інших типів: [які типи конфіденційних даних шукають](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="d639d-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  