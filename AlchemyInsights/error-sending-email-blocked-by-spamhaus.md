---
title: Помилка під час надсилання електронної пошти заблоковано SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: a16c998d2f289ea2da52454819f6677c405381a1
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/24/2019
ms.locfileid: "29495601"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="5e748-102">Помилка під час надсилання електронної пошти: клієнт хост заблоковано за допомогою Spamhaus</span><span class="sxs-lookup"><span data-stu-id="5e748-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="5e748-p101">IP-адресу, який надіслав повідомлення є блок списку належить [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Причини час заблоковано Spamhaus в розрізі порушення безпеки, скомпрометований машини обмін публічної адреси IP та Інтернет-провайдер (ISP) політики. Наведено можливі виправлення:</span><span class="sxs-lookup"><span data-stu-id="5e748-p101">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies. Possible fixes are:</span></span>
  
- <span data-ttu-id="5e748-106">Для заблокованого вхідних повідомлень до Office 365, де ви керуєте вихідного сервера електронної пошти вам потрібно визначити причину і видалити блок з сайту Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="5e748-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>
    
- <span data-ttu-id="5e748-p102">Для заблокованого вхідних повідомлень до Office 365, де джерело IP-адреса належить іншому користувачу власником адрес потрібно видалити блок з сайту Spamhaus. Якщо IP-адреси на список блок політики (PBL), власник може призначити різні статичної IP-адреси або видалити адресу від на PBL.</span><span class="sxs-lookup"><span data-stu-id="5e748-p102">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website. If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>
    
- <span data-ttu-id="5e748-p103">Для заблокованого вихідне повідомлення з вашого домену Office 365 ви можете отримувати цю помилку, якщо переадресовується через 3rd party службу. За допомогою інструмент пошук WHOIS для пошуку заблокованих IP адреса власника.</span><span class="sxs-lookup"><span data-stu-id="5e748-p103">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service. You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
    

