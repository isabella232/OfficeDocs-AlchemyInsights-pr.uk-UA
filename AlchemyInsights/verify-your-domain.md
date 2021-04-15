---
title: Перевірка домену
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 4a34de7fa2aaaae365cf4562d31590d4b5fb7544
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51771012"
---
# <a name="verify-your-domain"></a><span data-ttu-id="f77d2-102">Перевірка домену</span><span class="sxs-lookup"><span data-stu-id="f77d2-102">Verify your domain</span></span>

 <span data-ttu-id="f77d2-103">**Імовірно, запис не оновлено в Інтернеті.**</span><span class="sxs-lookup"><span data-stu-id="f77d2-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="f77d2-104">Зазвичай новий запис відображається лише за кілька хвилин, але іноді це може тривати кілька годин.</span><span class="sxs-lookup"><span data-stu-id="f77d2-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="f77d2-105">Якщо минуло вже минуло, переконайтеся, що точне значення скопійовано та вставлено в запис TXT для перевірки на хості DNS.</span><span class="sxs-lookup"><span data-stu-id="f77d2-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="f77d2-106">Одна з поширених проблем не включає частину запису "MS=".</span><span class="sxs-lookup"><span data-stu-id="f77d2-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="f77d2-107">Ми також потребуємо цього!</span><span class="sxs-lookup"><span data-stu-id="f77d2-107">We need that too!</span></span>

- <span data-ttu-id="f77d2-108">На деяких хостах DNS потрібно виконати додатковий крок, щоб зберегти файл зони (де зберігається запис DNS), щоб він оновлювався в Інтернеті.</span><span class="sxs-lookup"><span data-stu-id="f77d2-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="f77d2-109">Переконайтеся, що ви зберегли зміни, щоб корпорація Майкрософт могла переглянути та перевірити запис.</span><span class="sxs-lookup"><span data-stu-id="f77d2-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
