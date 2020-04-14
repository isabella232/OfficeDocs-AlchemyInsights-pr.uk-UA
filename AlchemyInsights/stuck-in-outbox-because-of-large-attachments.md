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
- "9002385"
- "4645"
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241273"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="b87fb-102">Виправлення повідомлень, які застрягли в папці "Вихідні"</span><span class="sxs-lookup"><span data-stu-id="b87fb-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="b87fb-103">Корпорація Майкрософт рекомендує, запуску, запустивши сценарій ["у мене виникають проблеми з надсиланням, отримання або пошуку повідомлень електронної пошти"](https://aka.ms/SaRA-OutlookSendReceive) з [підтримки Microsoft і відновлення помічника](https://diagnostics.office.com/#/) .</span><span class="sxs-lookup"><span data-stu-id="b87fb-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="b87fb-104">Коли повідомлення застрягне у папці "Вихідні", найімовірніше, це велике вкладення, або параметр "Надіслати відразу після підключення" не ввімкнуто.</span><span class="sxs-lookup"><span data-stu-id="b87fb-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="b87fb-105">**Видалити велике вкладення**</span><span class="sxs-lookup"><span data-stu-id="b87fb-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="b87fb-106">У програмі Outlook виберіть пункт **надсилання й отримання** > **роботи в автономному режимі**.</span><span class="sxs-lookup"><span data-stu-id="b87fb-106">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="b87fb-107">В області переходів виберіть " **вихідні**".</span><span class="sxs-lookup"><span data-stu-id="b87fb-107">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="b87fb-108">Звідси ви можете:</span><span class="sxs-lookup"><span data-stu-id="b87fb-108">From here, you can:</span></span> 
    - <span data-ttu-id="b87fb-109">Видаліть повідомлення (виділіть його та натисніть кнопку **Видалити**).</span><span class="sxs-lookup"><span data-stu-id="b87fb-109">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="b87fb-110">Перетягніть повідомлення до папки чернетки, двічі клацніть, щоб відкрити його, і видаліть вкладення, виберіть його, а потім виберіть **Видалити**).</span><span class="sxs-lookup"><span data-stu-id="b87fb-110">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="b87fb-111">Якщо з'являється повідомлення про помилку, яке говорить, що Outlook намагається передати повідомлення, закрийте Outlook.</span><span class="sxs-lookup"><span data-stu-id="b87fb-111">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="b87fb-112">Це може зайняти кілька хвилин, щоб вийти.</span><span class="sxs-lookup"><span data-stu-id="b87fb-112">It may take a few moments to exit.</span></span> <span data-ttu-id="b87fb-113">Якщо Outlook не закрито, натисніть сполучення клавіш CTRL + ALT + DELETE і виберіть **запустити диспетчер завдань**.</span><span class="sxs-lookup"><span data-stu-id="b87fb-113">If Outlook doesn't close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="b87fb-114">У диспетчері завдань виберіть вкладку **процеси** , прокрутіть униз до програми Outlook. exe і виберіть **завершити процес**.</span><span class="sxs-lookup"><span data-stu-id="b87fb-114">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="b87fb-115">Після того, як Outlook закривається, перезавантажте його і повторіть кроки 2 і 3.</span><span class="sxs-lookup"><span data-stu-id="b87fb-115">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="b87fb-116">Після видалення вкладення натисніть кнопку **Надіслати/отримати** > **роботу автономно** , щоб відновити роботу в Інтернеті.</span><span class="sxs-lookup"><span data-stu-id="b87fb-116">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="b87fb-117">Повідомлення також застрягають в папці "Вихідні" після натискання кнопки " **Надіслати**", але ви не підключені.</span><span class="sxs-lookup"><span data-stu-id="b87fb-117">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="b87fb-118">Натисніть **Надіслати/отримати** та подивіться на кнопку **Автономна робота** .</span><span class="sxs-lookup"><span data-stu-id="b87fb-118">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="b87fb-119">Якщо це синій, ви відключені.</span><span class="sxs-lookup"><span data-stu-id="b87fb-119">If it's blue, you're disconnected.</span></span> <span data-ttu-id="b87fb-120">Натисніть його, щоб з'єднатися (кнопка стає білим) і натисніть кнопку **відправити все**.</span><span class="sxs-lookup"><span data-stu-id="b87fb-120">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="b87fb-121">**Увімкнути надсилання одразу після підключення**</span><span class="sxs-lookup"><span data-stu-id="b87fb-121">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="b87fb-122">На вкладці "файл" натисніть кнопку **"Параметри**".</span><span class="sxs-lookup"><span data-stu-id="b87fb-122">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="b87fb-123">У діалоговому вікні Параметри Outlook натисніть кнопку " **Додатково**".</span><span class="sxs-lookup"><span data-stu-id="b87fb-123">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="b87fb-124">У розділі надсилання й отримання клацніть, щоб увімкнути **надсилання одразу після підключення**.</span><span class="sxs-lookup"><span data-stu-id="b87fb-124">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="b87fb-125">Натисніть кнопку **OK**.</span><span class="sxs-lookup"><span data-stu-id="b87fb-125">Click **OK**.</span></span>
 
<span data-ttu-id="b87fb-126">Для отримання докладної інформації див.:</span><span class="sxs-lookup"><span data-stu-id="b87fb-126">For full details, see:</span></span>
- [<span data-ttu-id="b87fb-127">Відео: надсилання або видалення застрягли електронної пошти</span><span class="sxs-lookup"><span data-stu-id="b87fb-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="b87fb-128">Електронна пошта залишається в папці "Вихідні", доки вручну не ініціювати операцію надсилання й отримання в Outlook</span><span class="sxs-lookup"><span data-stu-id="b87fb-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
