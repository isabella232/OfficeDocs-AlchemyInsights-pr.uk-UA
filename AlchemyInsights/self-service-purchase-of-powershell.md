---
title: Самостійне придбання PowerShell
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
- "3516"
ms.openlocfilehash: 48b5b0a1be1bc03d45a531a1093f18a3f750c37d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51797742"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="57468-102">Самостійне придбання PowerShell</span><span class="sxs-lookup"><span data-stu-id="57468-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="57468-103">Щоб використовувати модуль MSCommerce PowerShell, потрібно інсталювати його на пристрої з Windows 10 з TLS 1.2 (потрібні дозволи локального адміністратора).</span><span class="sxs-lookup"><span data-stu-id="57468-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="57468-104">Імпорт і підключення до модуля MSCommerce.</span><span class="sxs-lookup"><span data-stu-id="57468-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="57468-105">Коли з'явиться запит на вхід, знадобиться використовувати облікові дані ролі глобального або облікового адміністратора.</span><span class="sxs-lookup"><span data-stu-id="57468-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="57468-106">Якщо у вас немає протоколу TLS 1.2, під час спроби отримати або оновити політику може з'явитися таке повідомлення про помилку:</span><span class="sxs-lookup"><span data-stu-id="57468-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="57468-107">ErrorMessage – основне підключення закрито: під час надсилання сталася *неочікувана помилка.*</span><span class="sxs-lookup"><span data-stu-id="57468-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



