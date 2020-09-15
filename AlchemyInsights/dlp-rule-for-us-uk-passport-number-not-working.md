---
title: Правило DLP для паспорта США або Великобританії не працює
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679245"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="d682b-102">Проблеми з номерами паспорта DLP-US/UK</span><span class="sxs-lookup"><span data-stu-id="d682b-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="d682b-103">**Важливо**: у ці безпрецедентні часи ми докладаємо всіх зусиль до того, щоб служби SharePoint Online і OneDrive були завжди доступні. Докладні відомості надано у статті [Тимчасові коригування функцій SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="d682b-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="d682b-104">**Помилки DLP із паспортами US/UK**</span><span class="sxs-lookup"><span data-stu-id="d682b-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="d682b-105">У вас виникли проблеми з **запобіганням втрати даних (DLP)** , які не працюють для вмісту, що містить **паспорт ГРОМАДЯНИНА США або Великобританії** , коли використовується тип конфіденційної інформації DLP у O365?</span><span class="sxs-lookup"><span data-stu-id="d682b-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="d682b-106">Якщо це так, переконайтеся, що вміст містить потрібні відомості про те, що таке політика DLP шукає, коли вона обчислюється.</span><span class="sxs-lookup"><span data-stu-id="d682b-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="d682b-107">Наприклад, для паспорта " **номер для США/uk** ", настроєного на рівень впевненості в 75%, наведені нижче оцінки та мають виявлятися для показу правила.</span><span class="sxs-lookup"><span data-stu-id="d682b-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="d682b-108">**[Формат:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Дев'ять цифр</span><span class="sxs-lookup"><span data-stu-id="d682b-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nine digits</span></span>

- <span data-ttu-id="d682b-109">**[Візерунок:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Дев'ять послідовних цифр</span><span class="sxs-lookup"><span data-stu-id="d682b-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="d682b-110">**[Контрольна сума:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ні, немає контрольної суми</span><span class="sxs-lookup"><span data-stu-id="d682b-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="d682b-111">**[Визначення:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Політика DLP – 75% упевнений, що це тип конфіденційної інформації, якщо в безпосередній близькості від 300 символів:</span><span class="sxs-lookup"><span data-stu-id="d682b-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="d682b-112">Функція Func_usa_uk_passport знаходить вміст, який відповідає шаблону.</span><span class="sxs-lookup"><span data-stu-id="d682b-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="d682b-113">Виявлено ключове слово з Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="d682b-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="d682b-114">Наприклад, наведений нижче зразок буде тригер для **паспорта US/UK** : номер паспорта США 123456789</span><span class="sxs-lookup"><span data-stu-id="d682b-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="d682b-115">Щоб отримати докладні відомості про те, що потрібно знайти номер паспорта США або Великобританії для вашого вмісту, ознайомтеся з цим розділом у цій статті: [що таке типи конфіденційних даних, які шукають номер ПАСПОРТА США або Великобританії](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number) .</span><span class="sxs-lookup"><span data-stu-id="d682b-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span></span>
  
<span data-ttu-id="d682b-116">Використовуючи інший вбудований тип конфіденційної інформації, ознайомтеся з наведена нижче стаття для отримання відомостей про те, що необхідно для інших типів: [які типи важливих відомостей відображаються](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="d682b-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  