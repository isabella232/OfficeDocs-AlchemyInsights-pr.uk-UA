---
title: DLP правило для США / Великобританія номер паспорта, не працює
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
ms.openlocfilehash: bc91af8be58d49204f84cd7d22f481348af3c013
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529940"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="6883d-102">Проблеми з DLP - США / Великобританія паспорт чисел</span><span class="sxs-lookup"><span data-stu-id="6883d-102">Problems with DLP - US/UK Passport Numbers</span></span>

<span data-ttu-id="6883d-103">Виникають проблеми з **Запобігання втрати даних (DLP)** не працює для вмісту, який містить у **США / Великобританія номер паспорта** при використанні DLP конфіденційної інформації типу в O365?</span><span class="sxs-lookup"><span data-stu-id="6883d-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK Passport Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="6883d-104">Якщо це так, переконайтеся, що ваш зміст містить необхідну інформацію для що DLP політики шукає коли його оцінка.</span><span class="sxs-lookup"><span data-stu-id="6883d-104">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="6883d-105">Наприклад, у **США / номер паспорта Великобританії** політику настроєно з рівня довіри до 75%, наступні оцінюються і повинні бути виявлені правило викликати</span><span class="sxs-lookup"><span data-stu-id="6883d-105">For example, for a **US/UK Passport Number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="6883d-106">**[Формат:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Дев'яти цифр</span><span class="sxs-lookup"><span data-stu-id="6883d-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="6883d-107">**[Моделі:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Дев'ять послідовних цифр</span><span class="sxs-lookup"><span data-stu-id="6883d-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="6883d-108">**[Контрольна сума:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ні, немає не контрольної суми</span><span class="sxs-lookup"><span data-stu-id="6883d-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="6883d-109">**[Визначення:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP політика – 75% впевнені, що вона виявила цей тип конфіденційну інформацію if, в безпосередній близькості від 300 символів:</span><span class="sxs-lookup"><span data-stu-id="6883d-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="6883d-110">Функція Func_usa_uk_passport знаходить вміст, який відповідає візерунку.</span><span class="sxs-lookup"><span data-stu-id="6883d-110">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="6883d-111">Ключове слово з Keyword_passport знайшов.</span><span class="sxs-lookup"><span data-stu-id="6883d-111">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="6883d-112">Наприклад, у наведеному прикладі ініціює для в **США / номер паспорта Великобританії** політики: номер паспорта США 123456789</span><span class="sxs-lookup"><span data-stu-id="6883d-112">For example, the following sample would trigger for the **US/UK Passport Number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="6883d-113">Для отримання додаткової інформації про те, що потрібно для США / Великобританія номер паспорта, щоб бути виявлені для вашого змісту, дивіться наступний розділ у цій статті: [шукати те, що конфіденційних відомостей, надання яких США / номер паспорта Великобританії](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="6883d-113">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="6883d-114">За допомогою різних вбудований конфіденційної інформації типу, див. відомості про те, що вимагається для інших типів: [що конфіденційних відомостей, надання яких шукати](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="6883d-114">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  