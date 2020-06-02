---
title: Виправлення неполадок підказки безпеки для виявлення шахрайства перевірки
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 74913492a086de688067d588e95dd87e6946743b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505004"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="25358-102">Виправлення неполадок підказки безпеки для виявлення шахрайства перевірки</span><span class="sxs-lookup"><span data-stu-id="25358-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="25358-103">Якщо ви отримуєте безпеки відгук, який говорить: "відправник не вдалося наші перевірки шахрайства перевіряє і не може бути, хто вони здаються", то відправник не вдалося передати або DKIM або SPF перевірки автентичності.</span><span class="sxs-lookup"><span data-stu-id="25358-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="25358-104">Найкращий спосіб вирішити це для відправника, щоб авторизуватися.</span><span class="sxs-lookup"><span data-stu-id="25358-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="25358-105">Якщо відправник розсилає відправлення від вашого імені, вам необхідно авторизувати їх, додавши ІР-адресу відправника до запису SPF.</span><span class="sxs-lookup"><span data-stu-id="25358-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="25358-106">Перегляньте [Виправлення неполадок Червоної (підозрілої) підказки щодо безпеки для виявлення шахрайства](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) для отримання додаткових відомостей.</span><span class="sxs-lookup"><span data-stu-id="25358-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="25358-107">Ось деякі інші посилання, які можуть допомогти:</span><span class="sxs-lookup"><span data-stu-id="25358-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="25358-108">Як корпорація Майкрософт використовує Framework політики відправника (SPF), щоб запобігти спуфінгу</span><span class="sxs-lookup"><span data-stu-id="25358-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="25358-109">Налаштуйте SPF, щоб запобігти спуфінгу</span><span class="sxs-lookup"><span data-stu-id="25358-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
