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
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657950"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="55137-102">Налаштування Endpoint DLP</span><span class="sxs-lookup"><span data-stu-id="55137-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="55137-103">Microsoft Endpoint DLP дає змогу використовувати захист і моніторинг ЗВД для делікатної інформації на пристроях із Windows 10.</span><span class="sxs-lookup"><span data-stu-id="55137-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="55137-104">Після приєднання пристроїв до системи керування пристроями можна створити політики ЗВД, щоб застосовувати захисні дії до елементів.</span><span class="sxs-lookup"><span data-stu-id="55137-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="55137-105">Для моніторингу дій із делікатними елементами можна використовувати оглядач діяльності.</span><span class="sxs-lookup"><span data-stu-id="55137-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="55137-106">Докладні відомості див. в статті [Приєднання пристроїв до системи керування пристроями](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="55137-106">For more info, see [Onboarding devices into device management](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="55137-107">Щоб почати роботу з Endpoint DLP:</span><span class="sxs-lookup"><span data-stu-id="55137-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="55137-108">Переконайтеся, що у вас є відповідні ліцензії на продукти або передплачені ліцензії.</span><span class="sxs-lookup"><span data-stu-id="55137-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="55137-109">Докладні відомості див. в статті [Ліцензії на продукти або передплачені ліцензії](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="55137-109">For more info, see [SKU/subscriptions licensing](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="55137-110">Перевірте наявність дозволів, необхідних для вмикання керування пристроями, доступу до сторінки приєднання та вмикання або вимикання моніторингу пристроїв.</span><span class="sxs-lookup"><span data-stu-id="55137-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="55137-111">Докладні відомості див. в статті [Дозволи](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="55137-111">For more info, see [Permissions](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="55137-112">Приєднайте пристрої до системи керування пристроями за допомогою відповідної процедури.</span><span class="sxs-lookup"><span data-stu-id="55137-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="55137-113">Докладні відомості див. в статті [Приєднання пристроїв](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="55137-113">For more info, see [Onboarding devices](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="55137-114">Створіть політики ЗВД для захисту делікатних елементів.</span><span class="sxs-lookup"><span data-stu-id="55137-114">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="55137-115">Відомості див. в статті [Сценарії політики захисту від втрати даних у кінцевих точках](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="55137-115">For info, see [Endpoint DLP policy scenarios](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="55137-116">Додаткові відомості про Microsoft Endpoint DLP див. в статті [Відомості про Захист від втрати даних у кінцевих точках Microsoft 365 (підготовча версія)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="55137-116">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="55137-117">**Важливі кроки зі збирання даних у разі необхідності підтримки:**</span><span class="sxs-lookup"><span data-stu-id="55137-117">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="55137-118">[Завантажте аналізатор клієнта MDATP Preview.](https://aka.ms/betamdatpanalyzer)</span><span class="sxs-lookup"><span data-stu-id="55137-118">Download [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span></span>
1. <span data-ttu-id="55137-119">Запустіть інструмент як адміністратор із вікна командного рядка:</span><span class="sxs-lookup"><span data-stu-id="55137-119">Run the tool as Admin from the cmd window:</span></span>

    <span data-ttu-id="55137-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span><span class="sxs-lookup"><span data-stu-id="55137-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span></span>

1. <span data-ttu-id="55137-121">Коли з'явиться запит із запитом введіть кількість хвилин для збирання **трасування:**, введіть кількість хвилин, потрібних для запуску сценарію.</span><span class="sxs-lookup"><span data-stu-id="55137-121">When prompted with **Enter the number of minutes to collect traces:**, enter the number of minutes required to run the scenario.</span></span>
1. <span data-ttu-id="55137-122">Виконайте сценарій.</span><span class="sxs-lookup"><span data-stu-id="55137-122">Run the scenario.</span></span>

<span data-ttu-id="55137-123">Зберіть вихідні дані ZIP-файлу, щоб надати агенту підтримки.</span><span class="sxs-lookup"><span data-stu-id="55137-123">Collect the Zip file output to give to the Support agent.</span></span>
