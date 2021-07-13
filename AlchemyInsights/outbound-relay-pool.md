---
title: Вихідний пул реле
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/08/2021
ms.locfileid: "53381867"
---
# <a name="outbound-relay-pool"></a><span data-ttu-id="3a948-102">Вихідний пул реле</span><span class="sxs-lookup"><span data-stu-id="3a948-102">Outbound relay pool</span></span>

<span data-ttu-id="3a948-103">Корпорація Майкрософт вносив деякі зміни до конфігурації для пересилання або пересилання електронних листів Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3a948-103">Microsoft is making some changes to the configuration for relaying or forwarding email through Microsoft 365.</span></span> <span data-ttu-id="3a948-104">Повідомлення в певних сценаріях пересилаються або пересилаються через Microsoft 365 за допомогою спеціального пулу реле.</span><span class="sxs-lookup"><span data-stu-id="3a948-104">Messages in certain scenarios are forwarded or relayed through Microsoft 365 using a special relay pool.</span></span> <span data-ttu-id="3a948-105">Повідомлення, надіслані з використанням пулу реле, можуть поглянути на папку небажаної пошти одержувача.</span><span class="sxs-lookup"><span data-stu-id="3a948-105">Messages sent by using the relay pool could end up in recipient's junk mail folder.</span></span> <span data-ttu-id="3a948-106">Докладні відомості див. в цьому [звіті.](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span><span class="sxs-lookup"><span data-stu-id="3a948-106">For more information, see [Outbound delivery pools](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span></span>

<span data-ttu-id="3a948-107">Щоб уникнути використання пулу реле, переконайтеся, що переслані або релевовані повідомлення відповідають одній із таких умов:</span><span class="sxs-lookup"><span data-stu-id="3a948-107">To avoid a scenario using the relay pool, make sure that forwarded/relayed messages meet one of the following criteria:</span></span>

- <span data-ttu-id="3a948-108">Відправник вихідної пошти – це допустимий домен клієнта.</span><span class="sxs-lookup"><span data-stu-id="3a948-108">The outbound sender is an accepted domain of the tenant.</span></span>
- <span data-ttu-id="3a948-109">Структура політики відправника (SPF) передається, коли до Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3a948-109">Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.</span></span>
- <span data-ttu-id="3a948-110">DomainKeys Identified Mail (DKIM) на домені відправника P2 передає, коли повідомлення доходить Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3a948-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span></span>
 
<span data-ttu-id="3a948-111">Повідомлення, які відповідають наведеним вище умовам, не пересилаються через пул реле.</span><span class="sxs-lookup"><span data-stu-id="3a948-111">Messages that meet the above criteria are not relayed through the relay pool.</span></span>

<span data-ttu-id="3a948-112">Якщо запис MX для вашого домену вказує на стороння особу або локальний сервер, використовуйте розширене фільтрування, щоб перевірити перевірку SPF для вхідної електронної пошти та не надсилати електронну пошту через пул реле.</span><span class="sxs-lookup"><span data-stu-id="3a948-112">If the MX record for your domain is pointed to a third-party or on-premises server, use enhanced filtering to make sure the SPF validation is correct for inbound email and to avoid sending email through the relay pool.</span></span>

<span data-ttu-id="3a948-113">**Як можна дізнатися, чи впливає на нас пул реле?**</span><span class="sxs-lookup"><span data-stu-id="3a948-113">**How can we tell if we're impacted by the relay pool?**</span></span>

<span data-ttu-id="3a948-114">Якщо в пересланих або пересиланих електронних листах використовується одна з наведених вище умов, повідомлення не надсилатимуться через пул реле.</span><span class="sxs-lookup"><span data-stu-id="3a948-114">If your forwarded or relayed emails use one of the above criteria, messages won't be relayed through the relay pool.</span></span> <span data-ttu-id="3a948-115">Проте якщо повідомлення надсилається через пул реле, IP-адреса вихідного сервера входить до діапазону 40.95.0.0/16, а ім'я сервера вихідних підключень містить імена серверів вихідної пошти. </span><span class="sxs-lookup"><span data-stu-id="3a948-115">However, if a message is sent through a relay pool, the outbound server IP is in the 40.95.0.0/16 range and the outbound server name includes **rly** in the name.</span></span>

