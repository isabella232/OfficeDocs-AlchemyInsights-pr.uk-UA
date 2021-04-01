---
title: Установлення Microsoft Edge браузером за замовчуванням на пристрої macOS
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491819"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a><span data-ttu-id="02025-102">Установлення Microsoft Edge браузером за замовчуванням на пристрої macOS</span><span class="sxs-lookup"><span data-stu-id="02025-102">Set Microsoft Edge as the default browser on a macOS device</span></span>

<span data-ttu-id="02025-103">Скористаймося одним із цих двох способів, щоб зробити Microsoft Edge стандартним браузером:</span><span class="sxs-lookup"><span data-stu-id="02025-103">Use one of these two methods to set Microsoft Edge as the default browser:</span></span>

<span data-ttu-id="02025-104">Метод 1. Блимання пристрою зображенням macOS, де Microsoft Edge уже встановлено як стандартний браузер.</span><span class="sxs-lookup"><span data-stu-id="02025-104">Method 1: Flash the device with an image of macOS where Microsoft Edge has already been set as the default browser.</span></span>

<span data-ttu-id="02025-105">Метод 2. Установіть політику DefaultBrowserSettingEnabled, щоб користувач надав запит на встановлення Microsoft Edge браузером за замовчуванням.</span><span class="sxs-lookup"><span data-stu-id="02025-105">Method 2: Set the DefaultBrowserSettingEnabled policy to prompt the user to set Microsoft Edge as the default browser.</span></span>

<span data-ttu-id="02025-106">Будь-який спосіб дає змогу користувачу змінювати стандартний браузер.</span><span class="sxs-lookup"><span data-stu-id="02025-106">Either method allows a user to change the default browser.</span></span> <span data-ttu-id="02025-107">Тому ми радимо розгорнути політику DefaultBrowserSettingEnabled, навіть якщо ви використали метод 1.</span><span class="sxs-lookup"><span data-stu-id="02025-107">For this reason, we recommend that you deploy the DefaultBrowserSettingEnabled policy even if you used method 1.</span></span> <span data-ttu-id="02025-108">Якщо користувач змінив браузер за замовчуванням після розгортання політики, користувачу буде запропоновано повернути браузер за замовчуванням до Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="02025-108">If a user changes the default browser after the policy is deployed, the policy prompts the user to set the default browser back to Microsoft Edge.</span></span>
