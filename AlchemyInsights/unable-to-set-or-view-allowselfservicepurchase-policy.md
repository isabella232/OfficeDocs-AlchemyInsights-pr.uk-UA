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
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158582"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="a4330-102">Не вдається встановити або переглянути Дозволяєпослугуправила політики</span><span class="sxs-lookup"><span data-stu-id="a4330-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="a4330-103">Під час спроби встановити або переглянути Дозволяєполітики, з'являється таке повідомлення про помилку:</span><span class="sxs-lookup"><span data-stu-id="a4330-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="a4330-104">*HandleError: не вдалося отримати політику продукту з політикою політики "Дозволяєповідомлення", помилка-базове підключення закрито: сталася неочікувана помилка під час надсилання.*</span><span class="sxs-lookup"><span data-stu-id="a4330-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="a4330-105">Це може бути через стару версію транспортний рівень безпеки (TLS).</span><span class="sxs-lookup"><span data-stu-id="a4330-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="a4330-106">Щоб підключити службу MSCommerce, потрібно використовувати TLS 1,2 або більше.</span><span class="sxs-lookup"><span data-stu-id="a4330-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="a4330-107">Виконайте наведені нижче дії, щоб увімкнути/встановити протокол TLS 1,2, перевірте і повторіть спробу.</span><span class="sxs-lookup"><span data-stu-id="a4330-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="a4330-108">У командному рядку PowerShell (PS C:\) введіть таку команду, щоб УСТАНОВИТИ протокол TLS версії 1,2:</span><span class="sxs-lookup"><span data-stu-id="a4330-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="a4330-109">Перевірте, чи протокол TLS використовується, за допомогою такої команди:</span><span class="sxs-lookup"><span data-stu-id="a4330-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="a4330-110">Повторіть спробу отримати або оновити команди, за потреби.</span><span class="sxs-lookup"><span data-stu-id="a4330-110">Retry the Get or Update commands as needed.</span></span>

