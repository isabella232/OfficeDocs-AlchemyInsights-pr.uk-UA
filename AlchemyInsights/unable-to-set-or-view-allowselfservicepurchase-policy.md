---
title: Не вдається встановити або переглянути політику AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735220"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="315c4-102">Не вдається встановити або переглянути політику AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="315c4-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="315c4-103">Під час спроби встановити або переглянути політику AllowSelfServicePurchase з'являється таке повідомлення про помилку:</span><span class="sxs-lookup"><span data-stu-id="315c4-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="315c4-104">*HandleError: не вдалося отримати політику продукту з ідентифікатором політик "AllowSelfServicePurchase", Erritmessage-вихідне підключення було закрито: сталася неочікувана помилка на сторінці "надсилати".*</span><span class="sxs-lookup"><span data-stu-id="315c4-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="315c4-105">Це може бути пов'язано зі старою версією захисту транспортного шару (TLS).</span><span class="sxs-lookup"><span data-stu-id="315c4-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="315c4-106">Щоб підключитися до служби MSCommerce, потрібно використовувати протокол TLS 1,2 або новішої версії.</span><span class="sxs-lookup"><span data-stu-id="315c4-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="315c4-107">Виконайте наведені нижче дії, щоб увімкнути або настроїти протокол TLS для 1,2, перевірка та повторіть спробу.</span><span class="sxs-lookup"><span data-stu-id="315c4-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="315c4-108">У командному рядку PowerShell (PS C: \) Укажіть таку команду, щоб установити протокол TLS для версії 1,2:</span><span class="sxs-lookup"><span data-stu-id="315c4-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="315c4-109">Перевірте протокол TLS (-ів) у програмі, використовуючи таку команду:</span><span class="sxs-lookup"><span data-stu-id="315c4-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="315c4-110">Повторіть команду "отримати або оновити" за потреби.</span><span class="sxs-lookup"><span data-stu-id="315c4-110">Retry the Get or Update commands as needed.</span></span>

