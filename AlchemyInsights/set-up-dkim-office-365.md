---
title: Настроювання DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808728"
---
# <a name="setup-dkim"></a><span data-ttu-id="b5104-102">Настроювання DKIM</span><span class="sxs-lookup"><span data-stu-id="b5104-102">Setup DKIM</span></span>

<span data-ttu-id="b5104-103">У цій [статті наведено повні](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)вказівки з настроювання DKIM для користувацьких доменів у Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="b5104-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="b5104-104">Для **кожного** настроюваного домену потрібно створити **два** записи CNAME DKIM у службі розміщення DNS-доменів свого домену (зазвичай це реєстратор доменів).</span><span class="sxs-lookup"><span data-stu-id="b5104-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="b5104-105">Наприклад, contoso.com і fourthcoffee.com вимагають чотири записи CNAME DKIM: два для contoso.com і два для fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="b5104-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="b5104-106">Записи CNAME DKIM для **кожного** настроюваного домену використовують такі формати:</span><span class="sxs-lookup"><span data-stu-id="b5104-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="b5104-107">**Ім'я хоста**: `selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="b5104-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="b5104-108">**Указує на адресу або значення**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="b5104-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="b5104-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="b5104-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="b5104-110">**Ім'я хоста**: `selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="b5104-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="b5104-111">**Указує на адресу або значення**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="b5104-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="b5104-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="b5104-112">**TTL**: 3600</span></span>

   <span data-ttu-id="b5104-113">\<DomainGUID\> – це текст ліворуч `.mail.protection.outlook.com` у настроюваному ЗАПИСІ MX для настроюваного домену (наприклад, `contoso-com` для домену contoso.com).</span><span class="sxs-lookup"><span data-stu-id="b5104-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="b5104-114">\<InitialDomain\> – домен, який ви використовували під час реєстрації в Microsoft 365 (наприклад, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="b5104-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="b5104-115">Створивши записи CNAME для користувацьких доменів, виконайте наведені нижче вказівки.</span><span class="sxs-lookup"><span data-stu-id="b5104-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="b5104-116">муніципалітет.</span><span class="sxs-lookup"><span data-stu-id="b5104-116">a.</span></span> <span data-ttu-id="b5104-117">[Увійдіть у службу Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) за допомогою робочого або навчального облікового запису.</span><span class="sxs-lookup"><span data-stu-id="b5104-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="b5104-118">b.</span><span class="sxs-lookup"><span data-stu-id="b5104-118">b.</span></span> <span data-ttu-id="b5104-119">Виберіть піктограму запускача програм у лівому верхньому куті, а потім виберіть елемент **адміністратор**.</span><span class="sxs-lookup"><span data-stu-id="b5104-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="b5104-120">c.</span><span class="sxs-lookup"><span data-stu-id="b5104-120">c.</span></span> <span data-ttu-id="b5104-121">У нижній лівій частині вкладки розгорніть розділ **адміністратор** і натисніть кнопку **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="b5104-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="b5104-122">d.</span><span class="sxs-lookup"><span data-stu-id="b5104-122">d.</span></span> <span data-ttu-id="b5104-123">Перейдіть на сторінку **захист**  >  **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="b5104-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="b5104-124">e.</span><span class="sxs-lookup"><span data-stu-id="b5104-124">e.</span></span> <span data-ttu-id="b5104-125">Виберіть домен, а потім натисніть кнопку **Увімкнути** , щоб **підписати повідомлення для цього ДОМЕНУ з підписами DKIM**.</span><span class="sxs-lookup"><span data-stu-id="b5104-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="b5104-126">Повторіть цей крок для кожного настроюваного домену.</span><span class="sxs-lookup"><span data-stu-id="b5104-126">Repeat this step for each custom domain.</span></span>
