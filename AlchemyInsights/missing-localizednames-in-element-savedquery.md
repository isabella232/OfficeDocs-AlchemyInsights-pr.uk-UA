---
title: Відсутні "LocalizedNames" у елементі "збережений запит"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1739"
- "9000187"
ms.openlocfilehash: 4b25596ab68cf1723df4fa6a593cef5341c8ff16
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667143"
---
# <a name="missing-localizednames-in-element-savedquery"></a><span data-ttu-id="655fe-102">Відсутні "LocalizedNames" у елементі "збережений запит"</span><span class="sxs-lookup"><span data-stu-id="655fe-102">Missing 'LocalizedNames' in element 'savedquery'</span></span>

<span data-ttu-id="655fe-103">Щоб отримати довідку з відсутнього "LocalizedNames", [у розділі "елемент" збережений запит "має бути незавершений вміст. Очікувалося список можливих елементів: під час імпорту рішення Dynamics 365 виникає помилка "LocalizedNames](https://support.microsoft.com/help/4463330/the-element-savedquery-has-incomplete-content-list-of-possible-element)".</span><span class="sxs-lookup"><span data-stu-id="655fe-103">For help with missing 'LocalizedNames', see ["The element 'savedquery' has incomplete content. List of possible elements expected: 'LocalizedNames'" error occurs when importing a Dynamics 365 solution](https://support.microsoft.com/help/4463330/the-element-savedquery-has-incomplete-content-list-of-possible-element).</span></span>

<span data-ttu-id="655fe-104">Знайдіть спеціальні символи в імені подання, яке може спричинити цю проблему.</span><span class="sxs-lookup"><span data-stu-id="655fe-104">Look for special characters in the view name that might cause the issue.</span></span> <span data-ttu-id="655fe-105">Видаліть будь-які спеціальні символи в імені подання та експортуйте рішення ще раз.</span><span class="sxs-lookup"><span data-stu-id="655fe-105">Remove any special characters in the view name and export the solution again.</span></span>