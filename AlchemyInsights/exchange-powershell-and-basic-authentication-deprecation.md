---
title: Exchange PowerShell і припинення підтримки базової автентифікації
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
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813493"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="3bb8b-102">Exchange PowerShell і припинення підтримки базової автентифікації</span><span class="sxs-lookup"><span data-stu-id="3bb8b-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="3bb8b-103">Найновіші відомості про підключення до Exchange Online PowerShell без використання базової автентифікації [див. тут](https://aka.ms/exops-docs).</span><span class="sxs-lookup"><span data-stu-id="3bb8b-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span></span> <span data-ttu-id="3bb8b-104">Модуль PowerShell V2 не використовує базову автентифікацію.</span><span class="sxs-lookup"><span data-stu-id="3bb8b-104">The PowerShell V2 module does not use basic authentication.</span></span>

<span data-ttu-id="3bb8b-105">Зверніть увагу, що базову автентифікацію все одно потрібно ввімкнути на клієнтському комп'ютері.</span><span class="sxs-lookup"><span data-stu-id="3bb8b-105">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="3bb8b-106">У новому модулі PowerShell V2 використовується сучасна автентифікація, щоб установити підключення для ввімкнення всіх командлетів V2 на основі REST.</span><span class="sxs-lookup"><span data-stu-id="3bb8b-106">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="3bb8b-107">Крім того, можна отримати доступ до старіших командлетів PowerShell (RPS), створивши віддалений сеанс PowerShell.</span><span class="sxs-lookup"><span data-stu-id="3bb8b-107">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="3bb8b-108">Щоб створити сеанс RPS на комп'ютері з ОС Windows, необхідно ввімкнути базову автентифікацію WinRM на клієнтському комп’ютері, хоча в модулі використовується механізм сучасної автентифікації для автентифікації в службі.</span><span class="sxs-lookup"><span data-stu-id="3bb8b-108">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="3bb8b-109">Канал базової автентифікації WinRM використовується для транспортування маркерів сучасної автентифікації.</span><span class="sxs-lookup"><span data-stu-id="3bb8b-109">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="3bb8b-110">Якщо базову автентифікацію WinRM вимкнуто на клієнтському комп'ютері, нові командлети V2 продовжуватимуть працювати (на відміну від старіших командлетів RPS).</span><span class="sxs-lookup"><span data-stu-id="3bb8b-110">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
