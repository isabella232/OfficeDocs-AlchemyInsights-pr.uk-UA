---
title: Помилка під час надсилання електронної пошти заблоковано Спадхаус
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714279"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="d1ab1-102">Помилка під час надсилання електронної пошти: клієнт хоста заблоковано за допомогою Спадхаус</span><span class="sxs-lookup"><span data-stu-id="d1ab1-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="d1ab1-103">IP-адреса, яка надіслала повідомлення, знаходиться на блоці списку, який належить [Спадхаус](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="d1ab1-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="d1ab1-104">Причини, заблоковані Спаміхаус включають скомпрометовані облікові записи, скомпрометовані машини, що спільний доступ до публічної IP-адреси та політики інтернет-провайдера (ISP).</span><span class="sxs-lookup"><span data-stu-id="d1ab1-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="d1ab1-105">Можливі виправлення:</span><span class="sxs-lookup"><span data-stu-id="d1ab1-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="d1ab1-106">Для заблокованих вхідних повідомлень, де ви керуєте вихідним сервером електронної пошти, вам потрібно визначити причину і видалити блок з сайту Спадхаус.</span><span class="sxs-lookup"><span data-stu-id="d1ab1-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="d1ab1-107">Для заблокованих вхідних повідомлень, де Вихідна IP-адреса належить комусь іншому, власник адреси повинен видалити блок з веб-сайту Спадхаус.</span><span class="sxs-lookup"><span data-stu-id="d1ab1-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="d1ab1-108">Якщо IP-адресу, що знаходиться у списку політики блокування (PBL), власник може призначити іншу статичну IP-адресу або видалити адресу з PBL.</span><span class="sxs-lookup"><span data-stu-id="d1ab1-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="d1ab1-109">Для заблокованих вихідних повідомлень з вашого домену, підключеного до корпорації Майкрософт, ви можете отримати цю помилку, якщо повідомлення направляються через сторонній сервіс.</span><span class="sxs-lookup"><span data-stu-id="d1ab1-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="d1ab1-110">Ви можете скористатися інструментом підстановки WHOIS, щоб знайти власника заблокованої IP-адреси.</span><span class="sxs-lookup"><span data-stu-id="d1ab1-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
