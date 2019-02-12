---
title: 1554 помилку Winsock 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 9331a6c2b6e92a66fb97daf7dc5655ec320cba0f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29903138"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="60021-102">Помилку Winsock 10061</span><span class="sxs-lookup"><span data-stu-id="60021-102">Winsock error 10061</span></span>

<span data-ttu-id="60021-p101">Цей код помилки означає, що Office 365 не міг встановити TCP сокет (підключення) з кінцевого вузла. Найбільш вірогідною причиною цієї помилки є проблеми з конфігурацією брандмауера. Щоб усунути цю проблему, перевірте ці параметри:</span><span class="sxs-lookup"><span data-stu-id="60021-p101">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host. The most likely cause of this error is a problem with your firewall configuration. To fix the problem, check these settings:</span></span>
  
- <span data-ttu-id="60021-106">Перевірте конфігурацію брандмауера з інформацією в [Office 365 URL-адрес і Вихідна IP-адреса](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="60021-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>
    
- <span data-ttu-id="60021-107">Якщо повідомлення про помилку є специфічним для Exchange Online захисту (EOP), вам повинно було бути раніше повідомлення до зміни до [Exchange Online захисту IP-адрес](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="60021-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
    
- <span data-ttu-id="60021-108">Переконайтеся, що ваш інтернет-провайдер (ISP) не блокує порту.</span><span class="sxs-lookup"><span data-stu-id="60021-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>
    
- <span data-ttu-id="60021-109">Перевірте, чи смарт-хоста і цільової настройки сервера у вашому сполучні лінії.</span><span class="sxs-lookup"><span data-stu-id="60021-109">Verify the smart host and target server settings in your connectors.</span></span>
    
<span data-ttu-id="60021-110">Зверніть увагу, що Office 365 не блокує *Вхідні* підключення таким чином.</span><span class="sxs-lookup"><span data-stu-id="60021-110">Note that Office 365 doesn't block  *incoming*  connections in this manner.</span></span> 
  

