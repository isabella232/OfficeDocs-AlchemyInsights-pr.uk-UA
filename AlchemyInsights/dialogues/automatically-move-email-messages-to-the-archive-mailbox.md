---
title: Автоматичне переміщення повідомлень електронної пошти до поштової скриньки архіву
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
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527748"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a><span data-ttu-id="1b4b6-102">Автоматичне переміщення повідомлень електронної пошти до поштової скриньки архіву</span><span class="sxs-lookup"><span data-stu-id="1b4b6-102">Automatically move email messages to the archive mailbox</span></span>

<span data-ttu-id="1b4b6-103">Нижче описано, як настроїти політику для автоматичного переміщення старої електронної пошти користувача до архівної поштової скриньки.</span><span class="sxs-lookup"><span data-stu-id="1b4b6-103">Here's how to set up a policy to automatically move a user's old email to the archive mailbox:</span></span>

1. <span data-ttu-id="1b4b6-104">Перейдіть до архіву керування даними про [**відповідність & захисту**](https://go.microsoft.com/fwlink/p/?linkid=2077143)  >    >   , щоб переконатися, що для користувача активовано архівну поштову скриньку.</span><span class="sxs-lookup"><span data-stu-id="1b4b6-104">Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **Data governance** > **Archive** to verify an archive mailbox has been enabled for the user.</span></span> <span data-ttu-id="1b4b6-105">Якщо це не так, натисніть кнопку **Увімкнути** **, а потім** у вікні попередження.</span><span class="sxs-lookup"><span data-stu-id="1b4b6-105">If it hasn't, click **Enable** then **Yes** in the warning box.</span></span>
2. <span data-ttu-id="1b4b6-106">Перейдіть до [**центру адміністрування Exchange > керування дотриманням > позначок збереження**](https://go.microsoft.com/fwlink/?linkid=2059104).</span><span class="sxs-lookup"><span data-stu-id="1b4b6-106">Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span></span>
3. <span data-ttu-id="1b4b6-107">Виберіть піктограму +, а потім натисніть кнопку **автоматично застосуємо до всієї поштової скриньки**.</span><span class="sxs-lookup"><span data-stu-id="1b4b6-107">Choose the + icon then choose **automatically apply to entire mailbox**.</span></span>
4. <span data-ttu-id="1b4b6-108">Призначте ім'я тегу збереження та виберіть команду **Перехід до архіву**.</span><span class="sxs-lookup"><span data-stu-id="1b4b6-108">Assign a name to the retention tag, and choose **Move to Archive**.</span></span> <span data-ttu-id="1b4b6-109">Для періоду зберігання вкажіть потрібний час, наприклад 90 днів.</span><span class="sxs-lookup"><span data-stu-id="1b4b6-109">For the retention period, enter the time you want, such as 90 days.</span></span> <span data-ttu-id="1b4b6-110">Натисніть кнопку **Зберегти**.</span><span class="sxs-lookup"><span data-stu-id="1b4b6-110">Click **Save**.</span></span>
5. <span data-ttu-id="1b4b6-111">Тепер створіть політику збереження: натисніть кнопку **політики збереження**, виберіть піктограму, щоб додати нову політику.</span><span class="sxs-lookup"><span data-stu-id="1b4b6-111">Now create a retention policy: choose **retention policies**, choose the icon to add a new policy.</span></span>
6. <span data-ttu-id="1b4b6-112">Призначте ім'я політиці збереження, а потім натисніть і прокрутіть список, щоб переглянути та додати щойно створений тег збереження.</span><span class="sxs-lookup"><span data-stu-id="1b4b6-112">Assign a name to the retention policy, then click and scroll to find and add the retention tag you just created.</span></span> <span data-ttu-id="1b4b6-113">Натисніть кнопку **Зберегти**.</span><span class="sxs-lookup"><span data-stu-id="1b4b6-113">Click **Save**.</span></span>
7. <span data-ttu-id="1b4b6-114">Врешті-решт, застосуємо політику збереження до поштової скриньки користувача: ще в центрі адміністрування Exchange виберіть   >  **поштові скриньки** одержувачів.</span><span class="sxs-lookup"><span data-stu-id="1b4b6-114">Finally, apply the retention policy to the user's mailbox: still in the Exchange admin center, go to **recipients** > **mailboxes**.</span></span> <span data-ttu-id="1b4b6-115">Виберіть усі користувачі, до яких потрібно застосувати політику, а потім натисніть кнопку **редагувати** (піктограма олівця).</span><span class="sxs-lookup"><span data-stu-id="1b4b6-115">Choose all the users who you want to apply the policy to, then choose **Edit** (the pencil icon).</span></span>
8. <span data-ttu-id="1b4b6-116">У діалоговому вікні натисніть кнопку **функції поштової скриньки**.</span><span class="sxs-lookup"><span data-stu-id="1b4b6-116">In the dialog box, click **mailbox features**.</span></span> <span data-ttu-id="1b4b6-117">У розділі **політика збереження** застосуємо політику, яку ви щойно створили > **зберегти**.</span><span class="sxs-lookup"><span data-stu-id="1b4b6-117">Under **Retention policy**, apply the policy you just created > **Save**.</span></span>
9. <span data-ttu-id="1b4b6-118">Інструкції з застосування політики для всіх користувачів наведено в статті [застосування політики збереження до поштових скриньок](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span><span class="sxs-lookup"><span data-stu-id="1b4b6-118">For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span></span>
