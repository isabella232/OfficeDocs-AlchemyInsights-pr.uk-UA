---
title: Перевірка домену
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: d30f9b51c0164acd126f214a581ad6cec5eec04e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734327"
---
# <a name="verify-your-domain"></a><span data-ttu-id="240e6-102">Перевірка домену</span><span class="sxs-lookup"><span data-stu-id="240e6-102">Verify your domain</span></span>

 <span data-ttu-id="240e6-103">**Можливо, запис не оновлюється через Інтернет.**</span><span class="sxs-lookup"><span data-stu-id="240e6-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="240e6-104">Це зазвичай займе кілька хвилин, щоб ми могли бачити новий запис, але іноді може тривати кілька годин.</span><span class="sxs-lookup"><span data-stu-id="240e6-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="240e6-105">Якщо ви дочекалися, що вже давно, двічі перевірте, чи було скопійовано та вставлено точне значення в записі перевірки TXT на хості DNS.</span><span class="sxs-lookup"><span data-stu-id="240e6-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="240e6-106">Один із поширених проблем не включає в себе частину запису "MS =".</span><span class="sxs-lookup"><span data-stu-id="240e6-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="240e6-107">Ми потребуємо цього!</span><span class="sxs-lookup"><span data-stu-id="240e6-107">We need that too!</span></span>

- <span data-ttu-id="240e6-108">На деяких хостів DNS потрібно виконати додатковий крок, щоб зберегти файл зони (де зберігається запис DNS), щоб він оновлювався через Інтернет.</span><span class="sxs-lookup"><span data-stu-id="240e6-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="240e6-109">Переконайтеся, що ви зберегли свої зміни, щоб корпорація Майкрософт могла бачити та перевірити запис.</span><span class="sxs-lookup"><span data-stu-id="240e6-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
