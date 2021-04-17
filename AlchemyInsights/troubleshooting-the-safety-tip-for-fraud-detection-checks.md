---
title: Виправлення застрягання безпеки для перевірок шахрайства
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834752"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="a38aa-102">Виправлення застрягання безпеки для перевірок шахрайства</span><span class="sxs-lookup"><span data-stu-id="a38aa-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="a38aa-103">Якщо з'являється запевнення щодо безпечності, у якому сказано, що відправник не пройшов перевірку автентичності DKIM або SPF і не пройшов перевірку автентичності DKIM або SPF.</span><span class="sxs-lookup"><span data-stu-id="a38aa-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="a38aa-104">Найкращий спосіб вирішити цю проблему – авторизувати самостійно відправника.</span><span class="sxs-lookup"><span data-stu-id="a38aa-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="a38aa-105">Якщо відправник надсилає повідомлення від вашого імені, потрібно авторизувати їх, додавши IP-адресу відправника до запису SPF.</span><span class="sxs-lookup"><span data-stu-id="a38aa-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="a38aa-106">Докладні відомості див. в розділах Виправлення неполадок, пов'язаних із червоним [(підозрілим)](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) застряганням щодо безпечності для перевірки шахрайства.</span><span class="sxs-lookup"><span data-stu-id="a38aa-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="a38aa-107">Ось ще кілька посилань, які можуть допомогти:</span><span class="sxs-lookup"><span data-stu-id="a38aa-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="a38aa-108">Запобігання спуфінгам за допомогою структури політики відправників (SPF)</span><span class="sxs-lookup"><span data-stu-id="a38aa-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="a38aa-109">Настроювання SPF для запобігання спуфінгу</span><span class="sxs-lookup"><span data-stu-id="a38aa-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
