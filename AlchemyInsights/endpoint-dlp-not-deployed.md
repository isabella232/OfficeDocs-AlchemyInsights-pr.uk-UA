---
title: DLP кінцевої точки не розгорнуто на пристрої користувача
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731872"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a><span data-ttu-id="890ee-102">DLP кінцевої точки не розгорнуто на пристрої користувача</span><span class="sxs-lookup"><span data-stu-id="890ee-102">Endpoint DLP not deployed to user's device</span></span>

<span data-ttu-id="890ee-103">Якщо параметр захисту від втрати даних кінцевої точки (DLP) не застосовано до пристрою користувача, переконайтеся, що ви відповідаєте цим вимогам:</span><span class="sxs-lookup"><span data-stu-id="890ee-103">If the Endpoint data loss prevention (DLP) setting has not applied to a user's device, confirm you meet these requirements:</span></span>

- <span data-ttu-id="890ee-104">Windows 10 x64 збірки 1809 або пізнішої версії інстальовано на пристрої.</span><span class="sxs-lookup"><span data-stu-id="890ee-104">Windows 10 x64 build 1809 or later is installed on the device.</span></span>
- <span data-ttu-id="890ee-105">Інстальовано клієнт захисту від зловмисних програм версії 4.18.2009.7 або новішої.</span><span class="sxs-lookup"><span data-stu-id="890ee-105">Anti-malware client version 4.18.2009.7 or later is installed.</span></span>
- <span data-ttu-id="890ee-106">Це один **із** таких пристроїв:</span><span class="sxs-lookup"><span data-stu-id="890ee-106">The device is **one** of these:</span></span>
    
    - <span data-ttu-id="890ee-107">Azure Active Directory приєдналися (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="890ee-107">Azure Active Directory (Azure AD) joined</span></span>
    - <span data-ttu-id="890ee-108">Приєднано до гібридної служби Azure AD</span><span class="sxs-lookup"><span data-stu-id="890ee-108">Hybrid Azure AD joined</span></span>
    - <span data-ttu-id="890ee-109">AAD зареєстровано</span><span class="sxs-lookup"><span data-stu-id="890ee-109">AAD registered</span></span>

- <span data-ttu-id="890ee-110">Щоб виконати дії політики, переконайтеся, що microsoft Chromium Edge інстальовано на пристрої кінцевої точки.</span><span class="sxs-lookup"><span data-stu-id="890ee-110">To enforce policy actions, make sure Microsoft Chromium Edge browser is installed on the endpoint device.</span></span>

<span data-ttu-id="890ee-111">Додаткові вимоги до розгортання захисту від втрати даних кінцевої точки див. в цьому [документі.](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)</span><span class="sxs-lookup"><span data-stu-id="890ee-111">For additional requirements for deploying Endpoint DLP, see [Get started with Endpoint data loss prevention](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).</span></span>