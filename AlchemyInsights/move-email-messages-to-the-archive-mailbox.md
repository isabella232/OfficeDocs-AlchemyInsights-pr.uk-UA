---
title: Переміщення повідомлень електронної пошти до поштової скриньки архіву
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 35c11f1bfb7c61b28a64f0128c29ddf7b4fce939
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511061"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="93b68-102">Переміщення електронної пошти до поштової скриньки архіву</span><span class="sxs-lookup"><span data-stu-id="93b68-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="93b68-103">Переконайтеся, що **архівну поштову скриньку** ввімкнено.</span><span class="sxs-lookup"><span data-stu-id="93b68-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="93b68-104">Якщо ні, виконайте дії, описані в [цій статті](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) , щоб увімкнути архівну поштову скриньку.</span><span class="sxs-lookup"><span data-stu-id="93b68-104">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="93b68-105">Щоб автоматично архівувати повідомлення до поштової скриньки архіву, тег збереження з дією « **перемістити в архів** » має бути встановлено для **автоматичного застосування до всієї поштової скриньки (за промовчанням)**.</span><span class="sxs-lookup"><span data-stu-id="93b68-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="93b68-106">Використовуйте кроки тут, щоб створити тег: [Архів за замовчуванням](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="93b68-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="93b68-107">Далі додайте тег **архіву** до політики збереження.</span><span class="sxs-lookup"><span data-stu-id="93b68-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="93b68-108">У центрі адміністрування Exchange, виберіть політики **збереження** > додати **перемістити до архіву тег** політики > **зберегти**.</span><span class="sxs-lookup"><span data-stu-id="93b68-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="93b68-109">Тепер [призначте політику збереження](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) для конкретної поштової скриньки користувача.</span><span class="sxs-lookup"><span data-stu-id="93b68-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="93b68-110">Цю саму політику буде застосовано до **основної** та **архівної** поштової скриньки.</span><span class="sxs-lookup"><span data-stu-id="93b68-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="93b68-111">Можливо, необхідно примусити помічника з керованих папок (МЗС) для запуску та застосування нових параметрів до поштової скриньки користувача.</span><span class="sxs-lookup"><span data-stu-id="93b68-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="93b68-112">Виконайте таку команду під час [підключення до EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) , щоб запустити помічник із керованих папок для певної поштової скриньки:</span><span class="sxs-lookup"><span data-stu-id="93b68-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="93b68-113">Start-Управлінсья помічниці-тотожність<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="93b68-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="93b68-114">Для отримання додаткових відомостей про настроювання політики архівування зверніться до [налаштування політики архівування та видалення для поштових скриньок](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="93b68-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  