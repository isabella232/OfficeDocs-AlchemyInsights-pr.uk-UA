---
title: Використання Microsoft Inune для керування веб-доступом в Microsoft EDGE для iOS і Android
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003846"
- "6895"
ms.openlocfilehash: 4d6ab4df4ff9588ce5052421602e347c76c91c3f
ms.sourcegitcommit: a7952283882d341515623d5ae58eda14d0553449
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/10/2020
ms.locfileid: "49679612"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="af6d3-102">Використання Microsoft Inune для керування веб-доступом в Microsoft EDGE для iOS і Android</span><span class="sxs-lookup"><span data-stu-id="af6d3-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="af6d3-103">Microsoft EDGE для iOS і Android дає змогу користувачам переглядати веб-сторінки з кількох повністю окремих профілів.</span><span class="sxs-lookup"><span data-stu-id="af6d3-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="af6d3-104">Максимально доступні можливості захисту даних Microsoft 365 стають доступними, коли ви підписуєтеся на корпоративну мобільність + Security Suite, що включає в себе функції Microsoft InTune та Azure Active Directory, як-от умовний доступ.</span><span class="sxs-lookup"><span data-stu-id="af6d3-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="af6d3-105">Принаймні, ви захочете розгорнути політику умовного доступу, яка (1) дає змогу користувачам підключатися від мобільних пристроїв до Microsoft EDGE для iOS і Android і (2) впроваджує політику захисту від Microsoft Inune, яка забезпечує захищений режим перегляду.</span><span class="sxs-lookup"><span data-stu-id="af6d3-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="af6d3-106">Щоб зрозуміти, як можна використовувати умовний доступ і політики, див.:</span><span class="sxs-lookup"><span data-stu-id="af6d3-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="af6d3-107">Використання політик умовного доступу для служби Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="af6d3-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="af6d3-108">Створення політик захисту програми Microsoft Inune</span><span class="sxs-lookup"><span data-stu-id="af6d3-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="af6d3-109">Використовувати єдиний вхід для Azure Active Directory – підключені веб-програми в браузері, захищених політикою</span><span class="sxs-lookup"><span data-stu-id="af6d3-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="af6d3-110">Використання конфігурації програми для керування досвідом перегляду</span><span class="sxs-lookup"><span data-stu-id="af6d3-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="af6d3-111">Надання дозволу на використання лише робочих і навчальних облікових записів</span><span class="sxs-lookup"><span data-stu-id="af6d3-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="af6d3-112">Розгортання політик настроювання загальних програм</span><span class="sxs-lookup"><span data-stu-id="af6d3-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="af6d3-113">Розгортання політик конфігурації програм для захисту даних</span><span class="sxs-lookup"><span data-stu-id="af6d3-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="af6d3-114">Використання диспетчера кінцевих точок Microsoft для розгортання політик конфігурації програм</span><span class="sxs-lookup"><span data-stu-id="af6d3-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="af6d3-115">Щоб дізнатися, як отримати доступ до журналів керованих програм, перегляньте статтю [використання Microsoft EDGE для IOS і Android, щоб отримати доступ до журналів керованих програм](https://go.microsoft.com/fwlink/?linkid=2132578).</span><span class="sxs-lookup"><span data-stu-id="af6d3-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
