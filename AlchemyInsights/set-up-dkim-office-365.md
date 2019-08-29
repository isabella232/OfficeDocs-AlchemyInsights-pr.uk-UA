---
title: Установки DKIM у службі Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: dd908db6a4bc1739b3c1cff059387034d67e093d
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666285"
---
# <a name="setup-dkim-in-office-365"></a><span data-ttu-id="4a92d-102">Установки DKIM у службі Office 365</span><span class="sxs-lookup"><span data-stu-id="4a92d-102">Setup DKIM in Office 365</span></span>

<span data-ttu-id="4a92d-103">Повна інструкція з налаштування DKIM, настроюваних доменів у службі Office 365 використовуються [тут](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="4a92d-103">The complete instructions for configuring DKIM for custom domains in Office 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="4a92d-104">Для **кожного** користувача домену вам потрібно створити **два** записи DKIM CNAME вашого домену службі розміщення DNS (зазвичай Реєстратор домену).</span><span class="sxs-lookup"><span data-stu-id="4a92d-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="4a92d-105">Наприклад, contoso.com і fourthcoffee.com вимагає чотири записи DKIM CNAME: два на contoso.com і два для fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="4a92d-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="4a92d-106">На DKIM записи CNAME для **кожного** користувача домену за допомогою таких форматів:</span><span class="sxs-lookup"><span data-stu-id="4a92d-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="4a92d-107">**Ім'я хоста**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="4a92d-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="4a92d-108">**Пункту до значення або адресу**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="4a92d-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="4a92d-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="4a92d-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="4a92d-110">**Ім'я хоста**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="4a92d-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="4a92d-111">**Пункту до значення або адресу**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="4a92d-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="4a92d-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="4a92d-112">**TTL**: 3600</span></span>

   <span data-ttu-id="4a92d-113">\<DomainGUID\> текст ліворуч від `.mail.protection.outlook.com` в замовний запис MX для користувача домену (наприклад, `contoso-com` для домен contoso.com).</span><span class="sxs-lookup"><span data-stu-id="4a92d-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="4a92d-114">\<InitialDomain\> є домен, які використовувалися під час реєстрації в Office 365 (наприклад, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="4a92d-114">\<InitialDomain\> is the domain you used when you signed up for Office 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="4a92d-115">Після створення запису CNAME записів для настроюваних доменів, виконайте наступні інструкції.</span><span class="sxs-lookup"><span data-stu-id="4a92d-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="4a92d-116">муніципалітет.</span><span class="sxs-lookup"><span data-stu-id="4a92d-116">a.</span></span> <span data-ttu-id="4a92d-117">[Увійдіть до Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) з облікового запису роботи чи школи.</span><span class="sxs-lookup"><span data-stu-id="4a92d-117">[Sign in to Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="4a92d-118">b.</span><span class="sxs-lookup"><span data-stu-id="4a92d-118">b.</span></span> <span data-ttu-id="4a92d-119">Виберіть launcher піктограму у верхньому лівому і вибрати **адміністратора**.</span><span class="sxs-lookup"><span data-stu-id="4a92d-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="4a92d-120">c.</span><span class="sxs-lookup"><span data-stu-id="4a92d-120">c.</span></span> <span data-ttu-id="4a92d-121">У нижньому лівому навігації розширити **адміністратора** і виберіть **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="4a92d-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="4a92d-122">d.</span><span class="sxs-lookup"><span data-stu-id="4a92d-122">d.</span></span> <span data-ttu-id="4a92d-123">Перейдіть до **захисту** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="4a92d-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="4a92d-124">e.</span><span class="sxs-lookup"><span data-stu-id="4a92d-124">e.</span></span> <span data-ttu-id="4a92d-125">Виберіть домен а потім виберіть **Увімкнути** для **підписати повідомлення для цього домену з DKIM підписами**.</span><span class="sxs-lookup"><span data-stu-id="4a92d-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="4a92d-126">Повторіть цей крок для кожного користувача домену.</span><span class="sxs-lookup"><span data-stu-id="4a92d-126">Repeat this step for each custom domain.</span></span>
