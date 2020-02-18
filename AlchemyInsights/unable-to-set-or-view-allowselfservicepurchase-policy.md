---
title: Не вдається встановити або переглянути Дозволяєпослугуправила політики
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091786"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="5ab75-102">Не вдається встановити або переглянути Дозволяєпослугуправила політики</span><span class="sxs-lookup"><span data-stu-id="5ab75-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="5ab75-103">Під час спроби встановити або переглянути Дозволяєполітики, з'являється таке повідомлення про помилку:</span><span class="sxs-lookup"><span data-stu-id="5ab75-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="5ab75-104">*HandleError: не вдалося отримати політику продукту з політикою політики "Дозволяєповідомлення", помилка-базове підключення закрито: сталася неочікувана помилка під час надсилання.*</span><span class="sxs-lookup"><span data-stu-id="5ab75-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="5ab75-105">Це може бути через стару версію транспортний рівень безпеки (TLS).</span><span class="sxs-lookup"><span data-stu-id="5ab75-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="5ab75-106">Щоб підключити службу MSCommerce, потрібно використовувати TLS 1,2 або більше.</span><span class="sxs-lookup"><span data-stu-id="5ab75-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="5ab75-107">Виконайте наведені нижче дії, щоб увімкнути/встановити протокол TLS 1,2, перевірте і повторіть спробу.</span><span class="sxs-lookup"><span data-stu-id="5ab75-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="5ab75-108">У командному рядку PowerShell (PS C:\) введіть таку команду, щоб УСТАНОВИТИ протокол TLS версії 1,2:</span><span class="sxs-lookup"><span data-stu-id="5ab75-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    <span data-ttu-id="5ab75-109">\[Net. Послугменеджер _ сервісу]:: протокол безпеки = \[net. Ccctpcpeтип]:: Tls12</span><span class="sxs-lookup"><span data-stu-id="5ab75-109">\[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12</span></span>

2. <span data-ttu-id="5ab75-110">Перевірте, чи протокол TLS використовується, за допомогою такої команди:</span><span class="sxs-lookup"><span data-stu-id="5ab75-110">Verify the TLS protocol(s) in use, with the following command:</span></span>

    <span data-ttu-id="5ab75-111">\[Net. Послугменеджер]:: протокол безпеки</span><span class="sxs-lookup"><span data-stu-id="5ab75-111">\[Net.ServicePointManager]::SecurityProtocol</span></span> 

3. <span data-ttu-id="5ab75-112">Повторіть спробу отримати або оновити команди, за потреби.</span><span class="sxs-lookup"><span data-stu-id="5ab75-112">Retry the Get or Update commands as needed.</span></span>

