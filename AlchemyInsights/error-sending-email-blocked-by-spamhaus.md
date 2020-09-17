---
title: Помилка надсилання повідомлення електронної пошти, заблокованого за допомогою SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783824"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="21eb9-102">Помилка надсилання повідомлення електронної пошти: хост клієнта заблоковано за допомогою Spamhaus</span><span class="sxs-lookup"><span data-stu-id="21eb9-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="21eb9-103">IP-адреса, що надіслала повідомлення, належить до списку заблокованих у [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="21eb9-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="21eb9-104">Причини, які блокуються в Spamhaus, містять скомпрометовані облікові записи, що мають несанкціонований доступ до загальнодоступної IP-адреси, а також політики постачальника послуг Інтернету (ISP).</span><span class="sxs-lookup"><span data-stu-id="21eb9-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="21eb9-105">Можливі виправлення:</span><span class="sxs-lookup"><span data-stu-id="21eb9-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="21eb9-106">Для заблокованого вхідних повідомлень, у яких ви керуєте вихідним сервером електронної пошти, потрібно визначити причину та видалити блок із веб-сайту Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="21eb9-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="21eb9-107">Для заблокованого вхідних повідомлень, на які належить інший IP-адреса, власник адреси має видалити блок із веб-сайту Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="21eb9-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="21eb9-108">Якщо IP-адреса міститься в списку блок політики (ПБЛ), власник може призначати іншу статичну IP-адресу або видалити адресу від служби "Усі".</span><span class="sxs-lookup"><span data-stu-id="21eb9-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="21eb9-109">Для заблокованих вихідних повідомлень із домену, підключеного до корпорації Майкрософт, ви можете отримати цю помилку, якщо повідомлення спрямовуються через службу третьої сторони.</span><span class="sxs-lookup"><span data-stu-id="21eb9-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="21eb9-110">Щоб знайти заблоковану IP-адресу, можна скористатися засобом "Пошук за допомогою WHOIS".</span><span class="sxs-lookup"><span data-stu-id="21eb9-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
