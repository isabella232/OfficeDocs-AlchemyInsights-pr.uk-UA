---
title: Підтвердження домену
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 2c4d8e075d2cf7214b5ef005b856daf7fb0ed53c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710464"
---
# <a name="verify-your-domain"></a><span data-ttu-id="4b34b-102">Підтвердження домену</span><span class="sxs-lookup"><span data-stu-id="4b34b-102">Verify your domain</span></span>

 <span data-ttu-id="4b34b-103">**Можливо, запис не оновлено через Інтернет.**</span><span class="sxs-lookup"><span data-stu-id="4b34b-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="4b34b-104">Це зазвичай займе всього кілька хвилин для нас, щоб мати можливість побачити новий рекорд, але іноді це може зайняти до тих пір, як кілька годин.</span><span class="sxs-lookup"><span data-stu-id="4b34b-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="4b34b-105">Якщо ви вже давно чекали, двічі перевірте, що ви скопіювали та вставили точне значення в запис верифікації TXT на вашому DNS-хості.</span><span class="sxs-lookup"><span data-stu-id="4b34b-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="4b34b-106">Одна поширена проблема не в тому числі "MS =" частина запису.</span><span class="sxs-lookup"><span data-stu-id="4b34b-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="4b34b-107">Ми потребуємо цього теж!</span><span class="sxs-lookup"><span data-stu-id="4b34b-107">We need that too!</span></span>

- <span data-ttu-id="4b34b-108">У деяких хостів DNS потрібно зробити додатковий крок, щоб зберегти файл зони (де зберігається запис DNS), щоб він оновбув через Інтернет.</span><span class="sxs-lookup"><span data-stu-id="4b34b-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="4b34b-109">Переконайтеся, що ви зберегли зміни, тому корпорація Майкрософт може бачити та перевіряти запис.</span><span class="sxs-lookup"><span data-stu-id="4b34b-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
