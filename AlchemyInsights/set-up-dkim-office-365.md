---
title: Налаштування DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645693"
---
# <a name="setup-dkim"></a><span data-ttu-id="f1624-102">Налаштування DKIM</span><span class="sxs-lookup"><span data-stu-id="f1624-102">Setup DKIM</span></span>

<span data-ttu-id="f1624-103">Повні інструкції з налаштування DKIM для користувацьких доменів у Microsoft 365 є [тут](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="f1624-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="f1624-104">Для **кожного** настроюваного домену потрібно створити **два** записи DKIM CNAME у службі розміщення DNS вашого домену (зазвичай реєстратор доменів).</span><span class="sxs-lookup"><span data-stu-id="f1624-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="f1624-105">Наприклад, contoso.com і fourthcoffee.com потрібні чотири записи DKIM CNAME: два для contoso.com і два для fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="f1624-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="f1624-106">Записи DKIM CNAME для **кожного** настроюваного домену використовують такі формати:</span><span class="sxs-lookup"><span data-stu-id="f1624-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="f1624-107">**Ім'я хоста**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="f1624-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="f1624-108">**Вказує на адресу або значення**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="f1624-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="f1624-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="f1624-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="f1624-110">**Ім'я хоста**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="f1624-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="f1624-111">**Вказує на адресу або значення**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="f1624-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="f1624-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="f1624-112">**TTL**: 3600</span></span>

   <span data-ttu-id="f1624-113">\<Ідентифікатор\> домену — це текст зліва від `.mail.protection.outlook.com` настроюваного запису MX для настроюваного домену (наприклад, `contoso-com` для домену contoso.com).</span><span class="sxs-lookup"><span data-stu-id="f1624-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="f1624-114">\<У Ініціатодомені\> є домен, який використовувався під час підписування для Microsoft 365 (наприклад, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="f1624-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="f1624-115">Після створення записів CNAME для настроюваних доменів виконайте наведені нижче вказівки.</span><span class="sxs-lookup"><span data-stu-id="f1624-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="f1624-116">є.</span><span class="sxs-lookup"><span data-stu-id="f1624-116">a.</span></span> <span data-ttu-id="f1624-117">[увійдіть до Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) з робочим або навчальним обліковим записом.</span><span class="sxs-lookup"><span data-stu-id="f1624-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="f1624-118">B.</span><span class="sxs-lookup"><span data-stu-id="f1624-118">b.</span></span> <span data-ttu-id="f1624-119">Виберіть піктограму запуску програми у верхньому лівому куті та виберіть **адміністратор**.</span><span class="sxs-lookup"><span data-stu-id="f1624-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="f1624-120">C.</span><span class="sxs-lookup"><span data-stu-id="f1624-120">c.</span></span> <span data-ttu-id="f1624-121">У лівій частині навігації розгорніть **адміністратор** і виберіть **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="f1624-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="f1624-122">D.</span><span class="sxs-lookup"><span data-stu-id="f1624-122">d.</span></span> <span data-ttu-id="f1624-123">Перейти до **захисту** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="f1624-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="f1624-124">E.</span><span class="sxs-lookup"><span data-stu-id="f1624-124">e.</span></span> <span data-ttu-id="f1624-125">Виберіть домен, а потім виберіть **Увімкнути** для **підписування повідомлень для цього ДОМЕНУ з підписами DKIM**.</span><span class="sxs-lookup"><span data-stu-id="f1624-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="f1624-126">Повторіть цей крок для кожного настроюваного домену.</span><span class="sxs-lookup"><span data-stu-id="f1624-126">Repeat this step for each custom domain.</span></span>
