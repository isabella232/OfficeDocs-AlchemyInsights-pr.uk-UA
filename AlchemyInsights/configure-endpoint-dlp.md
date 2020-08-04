---
title: Настроювання кінцевої точки ЗВД
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 039c8f78c5896b66eab5763fb0bbddd3f0b06f2d
ms.sourcegitcommit: 1dada930649a2625eb6d15910b2bfd5e1e00e5b6
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/03/2020
ms.locfileid: "46556031"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="c6a22-102">Настроювання кінцевої точки ЗВД</span><span class="sxs-lookup"><span data-stu-id="c6a22-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="c6a22-103">Програма Microsoft endPoint ЗВД дає змогу розширити можливості захисту та моніторингу для конфіденційної інформації на пристроях Windows 10.</span><span class="sxs-lookup"><span data-stu-id="c6a22-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="c6a22-104">Після того, як пристрої, які сіли на пристрій керування, можна створити ЗВД політики для виконання захисних дій на елементи.</span><span class="sxs-lookup"><span data-stu-id="c6a22-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="c6a22-105">Провідник активності можна використовувати для відстеження активності чутливих елементів.</span><span class="sxs-lookup"><span data-stu-id="c6a22-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="c6a22-106">Для отримання додаткових [відомостей див.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)</span><span class="sxs-lookup"><span data-stu-id="c6a22-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="c6a22-107">Щоб почати з кінцевої точки ЗВД:</span><span class="sxs-lookup"><span data-stu-id="c6a22-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="c6a22-108">Переконайтеся, що у вас є відповідні номер ліцензії/передплати.</span><span class="sxs-lookup"><span data-stu-id="c6a22-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="c6a22-109">Для отримання додаткових [відомостей див.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing)</span><span class="sxs-lookup"><span data-stu-id="c6a22-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="c6a22-110">Перевірте дозволи, потрібні для ввімкнення керування пристроями, доступ до сторінки для публікування або Увімкнення/вимкнення моніторингу пристроїв.</span><span class="sxs-lookup"><span data-stu-id="c6a22-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="c6a22-111">Щоб отримати додаткові відомості, перегляньте [дозволи](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="c6a22-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="c6a22-112">На борту пристроїв у керування пристроями, дотримуючись процедури для ознайомлення.</span><span class="sxs-lookup"><span data-stu-id="c6a22-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="c6a22-113">Якщо у вас відсутня опція ознайомлення з пристроєм (попередній перегляд) у розділі **Параметри**відповідності M365, підтвердьте, що у вас є відповідна ліцензія та дозволи, які згадуються вище.</span><span class="sxs-lookup"><span data-stu-id="c6a22-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="c6a22-114">Докладніше про це у [пристрої](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="c6a22-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="c6a22-115">Створення ЗВД політики для захисту конфіденційних елементів.</span><span class="sxs-lookup"><span data-stu-id="c6a22-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="c6a22-116">Для отримання [відомостей див.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios)</span><span class="sxs-lookup"><span data-stu-id="c6a22-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="c6a22-117">Щоб отримати додаткові відомості про Microsoft кінцевої точки ЗВД, див. [відомості про microsoft 365 кінцевої точки попередження про втрату даних (попередній перегляд)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="c6a22-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>