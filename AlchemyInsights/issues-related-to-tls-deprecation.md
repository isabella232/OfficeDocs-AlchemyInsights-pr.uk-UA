---
title: Не вдається надіслати або отримати повідомлення електронної пошти з Office 365 через протокол TLS 1,0 і TLS 1,1 інвалідності
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747112"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a><span data-ttu-id="af590-102">Не вдається надіслати або отримати повідомлення електронної пошти з Office 365 через протокол TLS 1,0 і TLS 1,1 інвалідності</span><span class="sxs-lookup"><span data-stu-id="af590-102">Unable to send/receive email to/from Office 365 because of the TLS 1.0 and TLS 1.1 disablement</span></span>

<span data-ttu-id="af590-103">Як підтвердив повідомлення центру повідомлень MC229914, TLS 1,0 і TLS 1,1, Початок виконання для кінцевих точок потоку пошти Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="af590-103">As confirmed by the message center post MC229914, TLS 1.0 and TLS 1.1 deprecation started enforcing for Exchange Online mail flow endpoints.</span></span> <span data-ttu-id="af590-104">Незабаром Office 365 більше не прийматиме протокол TLS 1,0 і TLS 1,1 підключення до електронної пошти із зовнішніх джерел.</span><span class="sxs-lookup"><span data-stu-id="af590-104">Soon Office 365 will no longer accept TLS 1.0 and TLS 1.1 email connections from external sources.</span></span> <span data-ttu-id="af590-105">Крім того, Exchange Online ніколи не використовуватиме протокол TLS 1,0 або 1,1, щоб надсилати вихідні повідомлення електронної пошти.</span><span class="sxs-lookup"><span data-stu-id="af590-105">Also, Exchange Online will never use TLS 1.0 or 1.1 to send outbound email.</span></span> <span data-ttu-id="af590-106">Якщо ви зіткнулися з проблемами через TLS 1,0 або 1,1 інвалідності, може виникнути одна з таких помилок:</span><span class="sxs-lookup"><span data-stu-id="af590-106">If you are facing issues because of TLS 1.0 or 1.1 disablement, you might experience one of the following errors-</span></span>

- <span data-ttu-id="af590-107">Відправник отримує звіт про недоставку назад-' 421 4.4.2 з'єднання розірвано через помилку Sokeketerror '</span><span class="sxs-lookup"><span data-stu-id="af590-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="af590-108">Помилка в засобі перегляду черг локального сервера, на якому надсилається повідомлення електронної пошти офіцеру 365 – ' 421 4.4.2, через помилку «Сокіл»</span><span class="sxs-lookup"><span data-stu-id="af590-108">Error in the Queue Viewer of On-Premises server that is sending email to Officer 365- '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="af590-109">Помилка в журналі "Надіслати [протокол](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) з'єднувача" на сервері надсилання повідомлення електронної пошти до служби Office 365 – TLS не вдалося з помилкою Sokeketerror</span><span class="sxs-lookup"><span data-stu-id="af590-109">Error in Send connector [Protocol log](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) on the server sending email to Office 365- TLS negotiation failed with error SocketError</span></span>
- <span data-ttu-id="af590-110">Помилка в журналі "надсилати або отримувати сполучну лінію": "451 5.7.3 має видати спочатку команду STARTTLS"</span><span class="sxs-lookup"><span data-stu-id="af590-110">Error in Send or receive connector protocol log - '451 5.7.3 Must issue a STARTTLS command first'</span></span>

<span data-ttu-id="af590-111">Якщо у вас виникли наведені вище помилки, переконайтеся, що сервер, який надсилає або отримує повідомлення електронної пошти, має TLS 1,2 увімкнуто, перевіривши наведені нижче розділи реєстру.</span><span class="sxs-lookup"><span data-stu-id="af590-111">If you experience any of the above errors, please make sure the server that is sending or receiving email has TLS 1.2 enabled by checking the following registry keys-</span></span>

<span data-ttu-id="af590-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2 \ клієнт] **"Disablebydefault" = DWORD: 00000000 "увімкнено" = DWORD: 00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2 \ Server] **"Disablebydefault" = DWORD: 00000000 "увімкнено" = DWORD: 00000001**</span><span class="sxs-lookup"><span data-stu-id="af590-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span></span>

<span data-ttu-id="af590-113">Якщо ви вносите будь-які зміни в зазначених вище розділах реєстру, щоб увімкнути протокол TLS 1,2, перезавантажте сервер, щоб зміни набрали сили.</span><span class="sxs-lookup"><span data-stu-id="af590-113">If you make any change in the above registry keys to enable TLS 1.2, restart the server for the changes to take effect.</span></span> <span data-ttu-id="af590-114">Також переконайтеся, що інстальовано найновіші оновлення Windows і Exchange.</span><span class="sxs-lookup"><span data-stu-id="af590-114">Also make sure you have the latest Windows and Exchange updates installed.</span></span>

<span data-ttu-id="af590-115">Докладні відомості:</span><span class="sxs-lookup"><span data-stu-id="af590-115">For more information, see:</span></span>

- [<span data-ttu-id="af590-116">Посібник із сервера Exchange Server, частина 1: підготовка до TLS 1,2-спільнота Microsoft Tech</span><span class="sxs-lookup"><span data-stu-id="af590-116">Exchange Server TLS guidance, part 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [<span data-ttu-id="af590-117">Посібник із сервера Exchange Server частина 2: ввімкнення TLS 1,2 і визначення клієнтів, які не використовують її-спільнота Microsoft Tech</span><span class="sxs-lookup"><span data-stu-id="af590-117">Exchange Server TLS guidance Part 2: Enabling TLS 1.2 and Identifying Clients Not Using It - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [<span data-ttu-id="af590-118">Загальні відомості про сценарії електронної пошти, якщо версії TLS не можна узгодити з спільнотою Exchange Online – Microsoft Tech спільноти</span><span class="sxs-lookup"><span data-stu-id="af590-118">Understanding email scenarios if TLS versions cannot be agreed on with Exchange Online - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
