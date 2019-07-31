---
title: DLP не працює належним чином
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 1ea457bd69e7d545cf761a0be849695738b19d8b
ms.sourcegitcommit: d6ea6f4456a582559f27b34c0b9455a86a8e61f1
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/31/2019
ms.locfileid: "35941089"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="33937-102">DLP не працює належним чином</span><span class="sxs-lookup"><span data-stu-id="33937-102">DLP not working as expected</span></span>

<span data-ttu-id="33937-103">Виникли проблеми із **Запобігання втрати даних (DLP)** у службі Office 365, не працює належним чином?</span><span class="sxs-lookup"><span data-stu-id="33937-103">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="33937-104">Якщо це так, переконайтеся, що ваш **DLP політики** налаштовано правильно, і що дані містять що **DLP політики** є шукає, коли вона виконується оцінка.</span><span class="sxs-lookup"><span data-stu-id="33937-104">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
 <span data-ttu-id="33937-105">**Настроювання DLP**</span><span class="sxs-lookup"><span data-stu-id="33937-105">**Setting up DLP**</span></span>
  
<span data-ttu-id="33937-106">DLP політики дає змогу визначити та захисту конфіденційної інформації в організації.</span><span class="sxs-lookup"><span data-stu-id="33937-106">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="33937-107">Щоб налаштувати DLP політики, використовувати інформацію [тут](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="33937-107">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="33937-108">**Що шукати DLP політики**</span><span class="sxs-lookup"><span data-stu-id="33937-108">**What DLP policies look for**</span></span>
  
<span data-ttu-id="33937-109">При використанні **типи вбудованих конфіденційну інформацію** в Office 365 Безпека та відповідність вимогам центр, DLP політики Шукайте конкретні моделі та елементів при виявленні таких чутливих типів.</span><span class="sxs-lookup"><span data-stu-id="33937-109">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="33937-110">**Типи вбудованих конфіденційної інформації**</span><span class="sxs-lookup"><span data-stu-id="33937-110">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="33937-111">Докладніше про вбудованих чутливих типів і те, що політика DLP шукає при виявленні чутливі типу, дивіться: [шукати того, що вводить конфіденційну інформацію](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="33937-111">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="33937-112">**Типи настроюваних конфіденційної інформації**</span><span class="sxs-lookup"><span data-stu-id="33937-112">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="33937-113">Якщо ви маєте намір створити настроювані конфіденційну інформацію типів, використовувати наступну статтю відомості про те, як створити користувальницький чутливі тип: [Створити тип настроюваного конфіденційну інформацію](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="33937-113">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="33937-114">**Перевірити DLP політики**</span><span class="sxs-lookup"><span data-stu-id="33937-114">**Test a DLP policy**</span></span>

<span data-ttu-id="33937-115">Перевірити ваші дані за допомогою вбудованих і настроюваних конфіденційної інформації типу, скористайтеся параметром **перевірити тип** під **класифікацій** > **типи конфіденційну інформацію**.</span><span class="sxs-lookup"><span data-stu-id="33937-115">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="33937-116">Докладніше перегляньте [тест типи настроюваних конфіденційну інформацію](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="33937-116">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="33937-117">**Звіти**</span><span class="sxs-lookup"><span data-stu-id="33937-117">**Reports**</span></span>
  
- <span data-ttu-id="33937-118">Отримати конфіденційні дані insights з [звіти DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="33937-118">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="33937-119">Переглянути конкретні деталі заходу з [Звіт про інцидент](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="33937-119">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
