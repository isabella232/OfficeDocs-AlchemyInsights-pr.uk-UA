---
title: Налаштування Endpoint DLP
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402465"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="30f17-102">Налаштування Endpoint DLP</span><span class="sxs-lookup"><span data-stu-id="30f17-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="30f17-103">Microsoft Endpoint DLP дає змогу використовувати захист і моніторинг ЗВД для делікатної інформації на пристроях із Windows 10.</span><span class="sxs-lookup"><span data-stu-id="30f17-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="30f17-104">Після приєднання пристроїв до системи керування пристроями можна створити політики ЗВД, щоб застосовувати захисні дії до елементів.</span><span class="sxs-lookup"><span data-stu-id="30f17-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="30f17-105">Для моніторингу дій із делікатними елементами можна використовувати оглядач діяльності.</span><span class="sxs-lookup"><span data-stu-id="30f17-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="30f17-106">Докладні відомості див. в статті [Приєднання пристроїв до системи керування пристроями](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="30f17-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="30f17-107">Щоб почати роботу з Endpoint DLP:</span><span class="sxs-lookup"><span data-stu-id="30f17-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="30f17-108">Переконайтеся, що у вас є відповідні ліцензії на продукти або передплачені ліцензії.</span><span class="sxs-lookup"><span data-stu-id="30f17-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="30f17-109">Докладні відомості див. в статті [Ліцензії на продукти або передплачені ліцензії](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="30f17-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="30f17-110">Перевірте наявність дозволів, необхідних для вмикання керування пристроями, доступу до сторінки приєднання та вмикання або вимикання моніторингу пристроїв.</span><span class="sxs-lookup"><span data-stu-id="30f17-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="30f17-111">Докладні відомості див. в статті [Дозволи](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="30f17-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="30f17-112">Приєднайте пристрої до системи керування пристроями за допомогою відповідної процедури.</span><span class="sxs-lookup"><span data-stu-id="30f17-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="30f17-113">Якщо у вас немає параметра приєднання пристроїв (підготовча версія) в **Параметрах** Центру відповідності Microsoft 365, підтвердьте наявність відповідної ліцензії та дозволів, зазначених вище.</span><span class="sxs-lookup"><span data-stu-id="30f17-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="30f17-114">Докладні відомості див. в статті [Приєднання пристроїв](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="30f17-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="30f17-115">Створіть політики ЗВД для захисту делікатних елементів.</span><span class="sxs-lookup"><span data-stu-id="30f17-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="30f17-116">Відомості див. в статті [Сценарії політики захисту від втрати даних у кінцевих точках](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="30f17-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span></span>

<span data-ttu-id="30f17-117">Додаткові відомості про Microsoft Endpoint DLP див. в статті [Відомості про Захист від втрати даних у кінцевих точках Microsoft 365 (підготовча версія)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="30f17-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="30f17-118">**Важливі кроки зі збирання даних у разі необхідності підтримки:**</span><span class="sxs-lookup"><span data-stu-id="30f17-118">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="30f17-119">Завантажте аналізатор клієнта MDATP (підготовча версія) з [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span><span class="sxs-lookup"><span data-stu-id="30f17-119">Download MDATP Client Analyzer Preview from [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span></span>
2. <span data-ttu-id="30f17-120">Запустіть інструмент як адміністратор із вікна командного рядка:</span><span class="sxs-lookup"><span data-stu-id="30f17-120">Run the tool as Admin from the cmd window:</span></span>
3. <span data-ttu-id="30f17-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span><span class="sxs-lookup"><span data-stu-id="30f17-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span></span>
4. <span data-ttu-id="30f17-122">Коли з’явиться підказка "Введіть кількість хвилин для збирання результатів трасування: ", введіть кількість хвилин, необхідних для виконання сценарію</span><span class="sxs-lookup"><span data-stu-id="30f17-122">When prompted with “Enter the number of minutes to collect traces: ", enter the number of minutes that are required to run the scenario</span></span>
5. <span data-ttu-id="30f17-123">Виконайте сценарій</span><span class="sxs-lookup"><span data-stu-id="30f17-123">Run the scenario</span></span>

<span data-ttu-id="30f17-124">Зберіть вихідний ZIP-файл, який потрібно передати агенту підтримки.</span><span class="sxs-lookup"><span data-stu-id="30f17-124">Collect the Zip file output to be given to the Support agent.</span></span>
