---
title: Помилка під час надсилання електронної пошти заблоковано SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 39213f6f1b96c2bef9ea071f43c38766debf64d1
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527163"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="111f7-102">Помилка під час надсилання електронної пошти: клієнт хост заблоковано за допомогою Spamhaus</span><span class="sxs-lookup"><span data-stu-id="111f7-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="111f7-103">IP-адресу, який надіслав повідомлення є блок списку належить [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="111f7-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="111f7-104">Причини час заблоковано Spamhaus в розрізі порушення безпеки, скомпрометований машини обмін публічної адреси IP та Інтернет-провайдер (ISP) політики.</span><span class="sxs-lookup"><span data-stu-id="111f7-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="111f7-105">Наведено можливі виправлення:</span><span class="sxs-lookup"><span data-stu-id="111f7-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="111f7-106">Для заблокованого вхідних повідомлень до Office 365, де ви керуєте вихідного сервера електронної пошти вам потрібно визначити причину і видалити блок з сайту Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="111f7-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="111f7-107">Для заблокованого вхідних повідомлень до Office 365, де джерело IP-адреса належить іншому користувачу власником адрес потрібно видалити блок з сайту Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="111f7-107">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="111f7-108">Якщо IP-адреси на список блок політики (PBL), власник може призначити різні статичної IP-адреси або видалити адресу від на PBL.</span><span class="sxs-lookup"><span data-stu-id="111f7-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="111f7-109">Для заблокованого вихідне повідомлення з вашого домену Office 365 ви можете отримувати цю помилку, якщо переадресовується через 3rd party службу.</span><span class="sxs-lookup"><span data-stu-id="111f7-109">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="111f7-110">За допомогою інструмент пошук WHOIS для пошуку заблокованих IP адреса власника.</span><span class="sxs-lookup"><span data-stu-id="111f7-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
