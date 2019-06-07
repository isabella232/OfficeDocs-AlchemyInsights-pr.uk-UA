---
title: Установки DKIM у службі Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0f81fe02135f3d0901ffe5a26d7aa3dad70c3770
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765539"
---
# <a name="setup-dkim-in-office-365"></a><span data-ttu-id="6935e-102">Установки DKIM у службі Office 365</span><span class="sxs-lookup"><span data-stu-id="6935e-102">Setup DKIM in Office 365</span></span>

<span data-ttu-id="6935e-103">Повна інструкція з налаштування DKIM, настроюваних доменів у службі Office 365 використовуються [тут](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="6935e-103">The complete instructions for configuring DKIM for custom domains in Office 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="6935e-104">Для **кожного** користувача домену вам потрібно створити **два** записи DKIM CNAME вашого домену службі розміщення DNS (зазвичай Реєстратор домену).</span><span class="sxs-lookup"><span data-stu-id="6935e-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="6935e-105">Наприклад, contoso.com і fourthcoffee.com вимагає чотири записи DKIM CNAME: два на contoso.com і два для fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="6935e-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="6935e-106">На DKIM записи CNAME для **кожного** користувача домену за допомогою таких форматів:</span><span class="sxs-lookup"><span data-stu-id="6935e-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="6935e-107">**Ім'я хоста**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="6935e-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="6935e-108">**Пункту до значення або адресу**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="6935e-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="6935e-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="6935e-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="6935e-110">**Ім'я хоста**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="6935e-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="6935e-111">**Пункту до значення або адресу**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="6935e-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="6935e-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="6935e-112">**TTL**: 3600</span></span>

   <span data-ttu-id="6935e-113">\<DomainGUID\> текст ліворуч від `.mail.protection.outlook.com` в замовний запис MX для користувача домену (наприклад, `contoso-com` для домен contoso.com).</span><span class="sxs-lookup"><span data-stu-id="6935e-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="6935e-114">\<InitialDomain\> є домен, які використовувалися під час реєстрації в Office 365 (наприклад, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="6935e-114">\<InitialDomain\> is the domain you used when you signed up for Office 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="6935e-115">Після створення запису CNAME записів для настроюваних доменів, виконайте наступні інструкції.</span><span class="sxs-lookup"><span data-stu-id="6935e-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="6935e-116">муніципалітет.</span><span class="sxs-lookup"><span data-stu-id="6935e-116">a.</span></span> <span data-ttu-id="6935e-117">[Увійдіть до Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) з облікового запису роботи чи школи.</span><span class="sxs-lookup"><span data-stu-id="6935e-117">[Sign in to Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="6935e-118">b.</span><span class="sxs-lookup"><span data-stu-id="6935e-118">b.</span></span> <span data-ttu-id="6935e-119">Виберіть launcher піктограму у верхньому лівому і вибрати **адміністратора**.</span><span class="sxs-lookup"><span data-stu-id="6935e-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="6935e-120">c.</span><span class="sxs-lookup"><span data-stu-id="6935e-120">c.</span></span> <span data-ttu-id="6935e-121">У нижньому лівому навігації розширити **адміністратора** і виберіть **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="6935e-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="6935e-122">d.</span><span class="sxs-lookup"><span data-stu-id="6935e-122">d.</span></span> <span data-ttu-id="6935e-123">Перейдіть до **захисту** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="6935e-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="6935e-124">e.</span><span class="sxs-lookup"><span data-stu-id="6935e-124">e.</span></span> <span data-ttu-id="6935e-125">Виберіть домен а потім виберіть **Увімкнути** для **підписати повідомлення для цього домену з DKIM підписами**.</span><span class="sxs-lookup"><span data-stu-id="6935e-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="6935e-126">Повторіть цей крок для кожного користувача домену.</span><span class="sxs-lookup"><span data-stu-id="6935e-126">Repeat this step for each custom domain.</span></span>
