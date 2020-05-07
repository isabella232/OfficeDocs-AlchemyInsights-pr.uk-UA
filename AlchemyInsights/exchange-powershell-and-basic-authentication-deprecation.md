---
title: Exchange PowerShell і припинення підтримки базової автентифікації
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015710"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="beabc-102">Exchange PowerShell і припинення підтримки базової автентифікації</span><span class="sxs-lookup"><span data-stu-id="beabc-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="beabc-103">Найновіші відомості про підключення до Exchange Online PowerShell без використання базової автентифікації [див. тут](https://aka.ms/psbasicauth).</span><span class="sxs-lookup"><span data-stu-id="beabc-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/psbasicauth).</span></span>

<span data-ttu-id="beabc-104">Зверніть увагу, що базову автентифікацію все одно потрібно ввімкнути на клієнтському комп'ютері.</span><span class="sxs-lookup"><span data-stu-id="beabc-104">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="beabc-105">У новому модулі PowerShell V2 використовується сучасна автентифікація, щоб установити підключення для ввімкнення всіх командлетів V2 на основі REST.</span><span class="sxs-lookup"><span data-stu-id="beabc-105">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="beabc-106">Крім того, можна отримати доступ до старіших командлетів PowerShell (RPS), створивши віддалений сеанс PowerShell.</span><span class="sxs-lookup"><span data-stu-id="beabc-106">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="beabc-107">Щоб створити сеанс RPS на комп'ютері з ОС Windows, необхідно ввімкнути базову автентифікацію WinRM на клієнтському комп’ютері, хоча в модулі використовується механізм сучасної автентифікації для автентифікації в службі.</span><span class="sxs-lookup"><span data-stu-id="beabc-107">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="beabc-108">Канал базової автентифікації WinRM використовується для транспортування маркерів сучасної автентифікації.</span><span class="sxs-lookup"><span data-stu-id="beabc-108">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="beabc-109">Якщо базову автентифікацію WinRM вимкнуто на клієнтському комп'ютері, нові командлети V2 продовжуватимуть працювати (на відміну від старіших командлетів RPS).</span><span class="sxs-lookup"><span data-stu-id="beabc-109">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
