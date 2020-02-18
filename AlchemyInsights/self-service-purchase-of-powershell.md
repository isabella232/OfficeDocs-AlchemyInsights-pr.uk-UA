---
title: Купівля-самообслуговування PowerShell
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
- "3516"
ms.openlocfilehash: 5e47e08e3309b3d58908e10ee06021da00f230bb
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091785"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="18089-102">Купівля-самообслуговування PowerShell</span><span class="sxs-lookup"><span data-stu-id="18089-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="18089-103">Щоб скористатися модулем MSCommerce PowerShell, потрібно інсталювати його на пристрій Windows 10 із TLS 1,2 (необхідні дозволи локального адміністратора).</span><span class="sxs-lookup"><span data-stu-id="18089-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="18089-104">Імпорт і підключення до модуля MSCommerce.</span><span class="sxs-lookup"><span data-stu-id="18089-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="18089-105">Коли з'явиться запит на вхід, вам потрібно буде використовувати глобальні облікові дані або адміністратора для виставлення рахунків.</span><span class="sxs-lookup"><span data-stu-id="18089-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="18089-106">Якщо у вас немає TLS 1,2, може з'явитися таке повідомлення про помилку під час спроби отримати або оновити політику:</span><span class="sxs-lookup"><span data-stu-id="18089-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="18089-107">*Повідомлення помилки-базове підключення закрито: сталася неочікувана помилка*під час надсилання.</span><span class="sxs-lookup"><span data-stu-id="18089-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



