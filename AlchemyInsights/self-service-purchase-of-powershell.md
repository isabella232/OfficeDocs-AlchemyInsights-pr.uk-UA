---
title: Самостійне придбання PowerShell
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
- "3516"
ms.openlocfilehash: e6cc504ebef19cbe78f576d9b207fe2d951d0ef5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47739991"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="2aab4-102">Самостійне придбання PowerShell</span><span class="sxs-lookup"><span data-stu-id="2aab4-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="2aab4-103">Щоб скористатися модулем PowerShell MSCommerce, потрібно інсталювати його на пристрої з Windows 10 із протоколом TLS 1,2 (потрібен локальний дозвіл адміністратора).</span><span class="sxs-lookup"><span data-stu-id="2aab4-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="2aab4-104">Імпорт і підключення до модуля MSCommerce.</span><span class="sxs-lookup"><span data-stu-id="2aab4-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="2aab4-105">Коли з'явиться відповідний запит на вхід, потрібно буде використовувати облікові дані ролей глобального або облікового запису адміністратора.</span><span class="sxs-lookup"><span data-stu-id="2aab4-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="2aab4-106">Якщо у вас немає TLS 1,2, під час спроби отримати або оновити політику може з'явитися таке повідомлення про помилку:</span><span class="sxs-lookup"><span data-stu-id="2aab4-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="2aab4-107">*Erritmessage-вихідне підключення було закрито: під час надісланого повідомлення сталася неочікувана помилка*.</span><span class="sxs-lookup"><span data-stu-id="2aab4-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



