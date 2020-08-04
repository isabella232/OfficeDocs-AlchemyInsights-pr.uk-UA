---
title: Автоматичне очищення застарілі пристрої в InTune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555738"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="4a2b1-102">Автоматичне очищення застарілі пристрої в InTune</span><span class="sxs-lookup"><span data-stu-id="4a2b1-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="4a2b1-103">InTune дозволяє адміністратору налаштовувати проміжок часу між 90 і 270 днів, після чого застарілі пристрої видаляються з служби.</span><span class="sxs-lookup"><span data-stu-id="4a2b1-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="4a2b1-104">Цей параметр є організацією, і після активації негайно переходить в силу.</span><span class="sxs-lookup"><span data-stu-id="4a2b1-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="4a2b1-105">Усі пристрої, не перевірені на сервер InTune протягом періоду, що перевищує параметр, видаляються остаточно.</span><span class="sxs-lookup"><span data-stu-id="4a2b1-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="4a2b1-106">**Зверніть увагу** Лише MDM об'єкти пристрою мають право на цю дію очищення.</span><span class="sxs-lookup"><span data-stu-id="4a2b1-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="4a2b1-107">Виключені лише об'єкти пристрою.</span><span class="sxs-lookup"><span data-stu-id="4a2b1-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="4a2b1-108">Додаткову інформацію про те, коли пристрій стає придатним для видалення на основі пристрою очищення налаштування та її "стан":</span><span class="sxs-lookup"><span data-stu-id="4a2b1-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="4a2b1-109">Налаштування: **видалення пристроїв після останньої дати заїзду: так (певне значення (N) у днях, вказаних)**</span><span class="sxs-lookup"><span data-stu-id="4a2b1-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="4a2b1-110">На основі значення (N), настроєних у параметрі, служба InTune видаляє пристрій у вказані дні після того, як його було успішно виконано.</span><span class="sxs-lookup"><span data-stu-id="4a2b1-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="4a2b1-111">Налаштування: **видалення пристроїв після останньої дати заїзду: No**</span><span class="sxs-lookup"><span data-stu-id="4a2b1-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="4a2b1-112">180 днів після закінчення терміну дії сертифікату пристрою і не оновлюється, пристрій видаляється.</span><span class="sxs-lookup"><span data-stu-id="4a2b1-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="4a2b1-113">**Зверніть увагу** В обох випадках пристрій має успішно зареєстровано в InTune.</span><span class="sxs-lookup"><span data-stu-id="4a2b1-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="4a2b1-114">Реєстрація відбувається під час першого повернення пристрою за допомогою служби InTune.</span><span class="sxs-lookup"><span data-stu-id="4a2b1-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="4a2b1-115">Якщо пристрій успішно працює з InTune, але не стає InTune, зареєстрованих, пристрій видаляється 270 днів після реєстрації.</span><span class="sxs-lookup"><span data-stu-id="4a2b1-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="4a2b1-116">(90 днів, щоб позначити пристрій як відкликаний, а потім ще 180 днів, щоб видалити запис.)</span><span class="sxs-lookup"><span data-stu-id="4a2b1-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="4a2b1-117">Жоден механізм не існує в консолі InTune для встановлення дати закінчення терміну сертифікації пристрою для будь-якого пристрою.</span><span class="sxs-lookup"><span data-stu-id="4a2b1-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>