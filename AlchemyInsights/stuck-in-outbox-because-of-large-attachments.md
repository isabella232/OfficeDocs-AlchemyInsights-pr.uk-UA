---
title: Застряг у папці "Вихідні" з великих вкладень
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441326"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="28362-102">Виправлення повідомлень, які застрягли в папці "Вихідні"</span><span class="sxs-lookup"><span data-stu-id="28362-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="28362-103">Корпорація Майкрософт рекомендує, запуску, запустивши сценарій ["у мене виникають проблеми з надсиланням, отримання або пошуку повідомлень електронної пошти"](https://aka.ms/SaRA-OutlookSendReceive) з [підтримки Microsoft і відновлення помічника](https://diagnostics.office.com/#/) .</span><span class="sxs-lookup"><span data-stu-id="28362-103">We recommend that you start by running the scenario ["I’m having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="28362-104">Якщо повідомлення застрягне в папці "Вихідні", найімовірніше, це:</span><span class="sxs-lookup"><span data-stu-id="28362-104">When a message gets stuck in your Outbox, the most likely causes are:</span></span>
- <span data-ttu-id="28362-105">Великі вкладення.</span><span class="sxs-lookup"><span data-stu-id="28362-105">Large attachments.</span></span>
- <span data-ttu-id="28362-106">Параметр **Надіслати негайно, якщо підключення** не ввімкнуто.</span><span class="sxs-lookup"><span data-stu-id="28362-106">The **Send immediately when connected** option is not enabled.</span></span>

<span data-ttu-id="28362-107">Щоб видалити великі вкладення:</span><span class="sxs-lookup"><span data-stu-id="28362-107">To remove large attachments:</span></span> 

1. <span data-ttu-id="28362-108">У програмі Outlook виберіть пункт **надсилання й отримання** > **роботи в автономному режимі**.</span><span class="sxs-lookup"><span data-stu-id="28362-108">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="28362-109">В області переходів виберіть " **вихідні**".</span><span class="sxs-lookup"><span data-stu-id="28362-109">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="28362-110">Звідси ви можете:</span><span class="sxs-lookup"><span data-stu-id="28362-110">From here, you can:</span></span> 
    - <span data-ttu-id="28362-111">Видаліть повідомлення (виділіть його та натисніть кнопку **Видалити**).</span><span class="sxs-lookup"><span data-stu-id="28362-111">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="28362-112">Перетягніть повідомлення до папки чернетки, двічі клацніть, щоб відкрити його, і видаліть вкладення, виберіть його, а потім виберіть **Видалити**).</span><span class="sxs-lookup"><span data-stu-id="28362-112">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="28362-113">Якщо з'являється повідомлення про помилку, яке говорить, що Outlook намагається передати повідомлення, закрийте Outlook.</span><span class="sxs-lookup"><span data-stu-id="28362-113">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="28362-114">Це може зайняти кілька хвилин, щоб вийти.</span><span class="sxs-lookup"><span data-stu-id="28362-114">It may take a few moments to exit.</span></span> <span data-ttu-id="28362-115">Якщо Outlook не закрито, натисніть сполучення клавіш CTRL + ALT + DELETE і виберіть **запустити диспетчер завдань**.</span><span class="sxs-lookup"><span data-stu-id="28362-115">If Outlook doesn’t close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="28362-116">У диспетчері завдань виберіть вкладку **процеси** , прокрутіть униз до програми Outlook. exe і виберіть **завершити процес**.</span><span class="sxs-lookup"><span data-stu-id="28362-116">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="28362-117">Після того, як Outlook закривається, перезавантажте його і повторіть кроки 2 і 3.</span><span class="sxs-lookup"><span data-stu-id="28362-117">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="28362-118">Після видалення вкладення натисніть кнопку **Надіслати/отримати** > **роботу автономно** , щоб відновити роботу в Інтернеті.</span><span class="sxs-lookup"><span data-stu-id="28362-118">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="28362-119">Повідомлення також застрягають в папці "Вихідні" після натискання кнопки " **Надіслати**", але ви не підключені.</span><span class="sxs-lookup"><span data-stu-id="28362-119">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="28362-120">Натисніть **Надіслати/отримати** та подивіться на кнопку **Автономна робота** .</span><span class="sxs-lookup"><span data-stu-id="28362-120">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="28362-121">Якщо це синій, ви відключені.</span><span class="sxs-lookup"><span data-stu-id="28362-121">If it's blue, you're disconnected.</span></span> <span data-ttu-id="28362-122">Виберіть його для підключення (кнопка стає білою) і натисніть кнопку **Надіслати все**.</span><span class="sxs-lookup"><span data-stu-id="28362-122">Select it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="28362-123">Щоб увімкнути **надсилання одразу після підключення**:</span><span class="sxs-lookup"><span data-stu-id="28362-123">To enable **Send immediately when connected**:</span></span>
 
- <span data-ttu-id="28362-124">Виберіть пункт**Параметри** >   **файлу** > **Додатково**.</span><span class="sxs-lookup"><span data-stu-id="28362-124">Select **File** > **Options** >  **Advanced**.</span></span>
<span data-ttu-id="28362-125">У розділі **надсилання й отримання** виберіть **Надіслати відразу після підключення**, а потім натисніть **кнопку ОК**.</span><span class="sxs-lookup"><span data-stu-id="28362-125">In the **Send and receive** section, select **Send immediately when connected**, and then choose **OK**.</span></span>
 
<span data-ttu-id="28362-126">Для отримання докладної інформації див.:</span><span class="sxs-lookup"><span data-stu-id="28362-126">For full details see:</span></span>
- [<span data-ttu-id="28362-127">Відео: надсилання або видалення застрягли електронної пошти</span><span class="sxs-lookup"><span data-stu-id="28362-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="28362-128">Електронна пошта залишається в папці "Вихідні", доки вручну не ініціювати операцію надсилання й отримання в Outlook</span><span class="sxs-lookup"><span data-stu-id="28362-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
