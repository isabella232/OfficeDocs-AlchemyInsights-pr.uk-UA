---
title: Увімкнення вбудовування застарілих діалогових вікон для відкриття звітів
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814285"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="3d7f8-102">Увімкнення вбудовування застарілих діалогових вікон для відкриття звітів</span><span class="sxs-lookup"><span data-stu-id="3d7f8-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="3d7f8-103">**Ознака**</span><span class="sxs-lookup"><span data-stu-id="3d7f8-103">**Symptom**</span></span>

<span data-ttu-id="3d7f8-104">Користувачам не вдається відкрити звіти.</span><span class="sxs-lookup"><span data-stu-id="3d7f8-104">Users are unable to open reports.</span></span> <span data-ttu-id="3d7f8-105">"Сталася помилка.</span><span class="sxs-lookup"><span data-stu-id="3d7f8-105">"Something has gone wrong.</span></span> <span data-ttu-id="3d7f8-106">Перевірте технічні відомості, щоб дізнатися більше".</span><span class="sxs-lookup"><span data-stu-id="3d7f8-106">Check technical details for more details."</span></span>

<span data-ttu-id="3d7f8-107">**Причина**</span><span class="sxs-lookup"><span data-stu-id="3d7f8-107">**Cause**</span></span>

<span data-ttu-id="3d7f8-108">Не вдається завантажити звіти в UCI з помилкою "Дескриптор форми має Null-значення або не визначено".</span><span class="sxs-lookup"><span data-stu-id="3d7f8-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="3d7f8-109">Для звітів в UCI і надалі потрібні застарілі діалогові вікна, тому в системі клієнта має бути ввімкнуто функцію *allowlegacydialogsembedding.*</span><span class="sxs-lookup"><span data-stu-id="3d7f8-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="3d7f8-110">**Вирішення**</span><span class="sxs-lookup"><span data-stu-id="3d7f8-110">**Solution**</span></span>

1. <span data-ttu-id="3d7f8-111">Виберіть Параметри **>адміністрування > системних параметрів > вкладці Загальні.**</span><span class="sxs-lookup"><span data-stu-id="3d7f8-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="3d7f8-112">Установіть для параметра "Дозволити вбудовування певних застарілих діалогових вікон у клієнті браузера уніфікованого інтерфейсу" **значення Так.**</span><span class="sxs-lookup"><span data-stu-id="3d7f8-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
