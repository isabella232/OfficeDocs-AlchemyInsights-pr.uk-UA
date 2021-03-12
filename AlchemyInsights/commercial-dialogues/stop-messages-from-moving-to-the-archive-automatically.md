---
title: Автоматичне вимкнення повідомлень від переходу до архіву
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 2cb3e29dfd4f422e946b7887d4d44f373ff03794
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749816"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="e421a-102">Автоматичне вимкнення повідомлень від переходу до архіву</span><span class="sxs-lookup"><span data-stu-id="e421a-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="e421a-103">Якщо ви використовуєте політику збереження, ви можете змінити вік збереження в цій політиці, щоб вимкнути автоматичне архівування повідомлень.</span><span class="sxs-lookup"><span data-stu-id="e421a-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="e421a-104">Ось як це зробити.</span><span class="sxs-lookup"><span data-stu-id="e421a-104">Here's how:</span></span>

1. <span data-ttu-id="e421a-105">У [центрі адміністрування Exchange](https://go.microsoft.com/fwlink/?linkid=2059104)виберіть Теги збереження **відповідності**  >  .</span><span class="sxs-lookup"><span data-stu-id="e421a-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="e421a-106">Знайдіть тег збереження для переміщення до архіву.</span><span class="sxs-lookup"><span data-stu-id="e421a-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="e421a-107">У тегу збереження змініть період збереження (період архівування), щоб **ніколи не** зупиняти елементи автоматичного архівації за допомогою політики збереження.</span><span class="sxs-lookup"><span data-stu-id="e421a-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="e421a-108">Це змінить параметри архівації для всіх поштових скриньок, до яких застосовано цей тег збереження.</span><span class="sxs-lookup"><span data-stu-id="e421a-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>
