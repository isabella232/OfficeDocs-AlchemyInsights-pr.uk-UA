---
title: Переміщення повідомлень електронної пошти до поштової скриньки архіву
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799801"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="aac63-102">Переміщення електронної пошти до поштової скриньки архіву</span><span class="sxs-lookup"><span data-stu-id="aac63-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="aac63-103">Якщо ви хочете, щоб ми могли виконати автоматичні перевірки для наведених нижче параметрів, натисніть кнопку назад, < – угорі цієї сторінки, а потім введіть адресу електронної пошти користувача, у якого виникли проблеми з переміщенням електронної пошти до поштової скриньки архіву.</span><span class="sxs-lookup"><span data-stu-id="aac63-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="aac63-104">Переконайтеся, що активовано **поштову скриньку архіву** .</span><span class="sxs-lookup"><span data-stu-id="aac63-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="aac63-105">Якщо ні, виконайте кроки, описані в [цій статті](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) , щоб активувати поштову скриньку архіву.</span><span class="sxs-lookup"><span data-stu-id="aac63-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="aac63-106">Щоб автоматично архівувати повідомлення до архівної поштової скриньки, тег збереження з дією " **Перехід до архівування** " має бути настроєно **автоматично до всієї поштової скриньки (за замовчуванням)**.</span><span class="sxs-lookup"><span data-stu-id="aac63-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="aac63-107">У цій статті описано, як створити тег: [Тег архіву за замовчуванням](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="aac63-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="aac63-108">Потім додайте тег **архіву** до політики збереження.</span><span class="sxs-lookup"><span data-stu-id="aac63-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="aac63-109">У центрі адміністрування Exchange виберіть **політики збереження** > додати **тег "Перехід до архіву** " до політики > " **зберегти**".</span><span class="sxs-lookup"><span data-stu-id="aac63-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="aac63-110">Тепер [призначте політику збереження](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) до поштової скриньки певного користувача.</span><span class="sxs-lookup"><span data-stu-id="aac63-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="aac63-111">Цю саму політику буде застосовано до **основної** та **архівної** поштової скриньки.</span><span class="sxs-lookup"><span data-stu-id="aac63-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="aac63-112">Можливо, знадобиться примусово використовувати помічник із керованих папок (МЗС) для запуску та застосування нових настройок до поштової скриньки користувача.</span><span class="sxs-lookup"><span data-stu-id="aac63-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="aac63-113">Щоб запустити помічник із керованих папок для певної поштової скриньки, виконайте таку команду, коли [підключаєтеся до EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) .</span><span class="sxs-lookup"><span data-stu-id="aac63-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="aac63-114">Початок-ManagedFolderAssistant-ідентичність <name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="aac63-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="aac63-115">Докладні відомості про настроювання політики архівування наведено в статті [Настроювання політики архівування та видалення для поштових скриньок](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="aac63-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  