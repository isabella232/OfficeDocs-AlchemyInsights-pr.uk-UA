---
title: Не вдається встановити або переглянути політику AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826112"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="0e6eb-102">Не вдається встановити або переглянути політику AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="0e6eb-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="0e6eb-103">Під час спроби встановити або переглянути політику AllowSelfServicePurchase з'являється таке повідомлення про помилку:</span><span class="sxs-lookup"><span data-stu-id="0e6eb-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="0e6eb-104">*HandleError: не вдалося отримати політику продукту за допомогою PolicyId "AllowSelfServicePurchase", ErrorMessage – основне підключення закрито: під час надсилання сталася неочікувана помилка.*</span><span class="sxs-lookup"><span data-stu-id="0e6eb-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="0e6eb-105">Причиною цього може бути старіша версія протоколу TLS.</span><span class="sxs-lookup"><span data-stu-id="0e6eb-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="0e6eb-106">Щоб підключити службу MSCommerce, потрібно використовувати TLS 1.2 або більше.</span><span class="sxs-lookup"><span data-stu-id="0e6eb-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="0e6eb-107">Щоб увімкнути або встановити протокол TLS 1.2, перевірити та повторити спробу, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="0e6eb-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="0e6eb-108">У командному рядку PowerShell (PS C: введіть таку команду, щоб установити протокол \) TLS версії 1.2:</span><span class="sxs-lookup"><span data-stu-id="0e6eb-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="0e6eb-109">Перевірте використовувані протоколи TLS за допомогою такої команди:</span><span class="sxs-lookup"><span data-stu-id="0e6eb-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="0e6eb-110">За потреби повторіть ці команди: Отримати або Оновити.</span><span class="sxs-lookup"><span data-stu-id="0e6eb-110">Retry the Get or Update commands as needed.</span></span>

