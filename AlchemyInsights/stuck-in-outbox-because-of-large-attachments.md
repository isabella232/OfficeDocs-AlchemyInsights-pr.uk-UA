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
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232651"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="8ef4b-102">Виправлення повідомлень, які застрягли в папці "Вихідні"</span><span class="sxs-lookup"><span data-stu-id="8ef4b-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="8ef4b-103">Корпорація Майкрософт рекомендує, запуску за допомогою сценарію ["у мене проблеми з надсилання, отримання або пошуку повідомлень електронної пошти"](https://aka.ms/SaRA-OutlookSendReceive) від [служби підтримки Microsoft і відновлення помічника](https://diagnostics.office.com/#/) на проблемному комп'ютері.</span><span class="sxs-lookup"><span data-stu-id="8ef4b-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool on the affected machine.</span></span>

<span data-ttu-id="8ef4b-104">Коли повідомлення застрягне у папці "Вихідні", найімовірніше, це велике вкладення, або параметр "Надіслати відразу після підключення" не ввімкнуто.</span><span class="sxs-lookup"><span data-stu-id="8ef4b-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="8ef4b-105">**Видалити велике вкладення**</span><span class="sxs-lookup"><span data-stu-id="8ef4b-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="8ef4b-106">Натисніть кнопку **надсилання й отримання** > **роботи в автономному режимі**.</span><span class="sxs-lookup"><span data-stu-id="8ef4b-106">Click **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="8ef4b-107">В області переходів клацніть " **вихідні**".</span><span class="sxs-lookup"><span data-stu-id="8ef4b-107">In the navigation pane, click **Outbox**.</span></span> <span data-ttu-id="8ef4b-108">Звідси ви можете:</span><span class="sxs-lookup"><span data-stu-id="8ef4b-108">From here, you can:</span></span> 
    - <span data-ttu-id="8ef4b-109">Видалити повідомлення.</span><span class="sxs-lookup"><span data-stu-id="8ef4b-109">Delete the message.</span></span> <span data-ttu-id="8ef4b-110">Просто виберіть його і натисніть кнопку **Видалити**.</span><span class="sxs-lookup"><span data-stu-id="8ef4b-110">Just select it and click **Delete**.</span></span>
    - <span data-ttu-id="8ef4b-111">Перетягніть повідомлення до **папки чернетки**, двічі клацніть, щоб відкрити повідомлення та видаліть вкладення (клацніть його та натисніть кнопку **Видалити**).</span><span class="sxs-lookup"><span data-stu-id="8ef4b-111">Drag the message to your **drafts folder**, double-click to open the message, and delete the attachment (click it and click **Delete**).</span></span>
3. <span data-ttu-id="8ef4b-112">Якщо під час спроби передавання повідомлення сталася помилка, закрийте програму Outlook.</span><span class="sxs-lookup"><span data-stu-id="8ef4b-112">If an error tells you Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="8ef4b-113">Це може зайняти кілька хвилин, щоб вийти.</span><span class="sxs-lookup"><span data-stu-id="8ef4b-113">It may take a few moments to exit.</span></span> <span data-ttu-id="8ef4b-114">Якщо Outlook не закрито, натисніть **сполучення клавіш CTRL + ALT + DELETE** і натисніть **запустити диспетчер завдань**.</span><span class="sxs-lookup"><span data-stu-id="8ef4b-114">If Outlook doesn't close, press **Ctrl+Alt+Delete** and click **Start Task Manager**.</span></span> <span data-ttu-id="8ef4b-115">У диспетчері завдань виберіть вкладку **процеси** , прокрутіть униз до програми Outlook. exe і натисніть кнопку **завершити процес**.</span><span class="sxs-lookup"><span data-stu-id="8ef4b-115">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and click **End Process**.</span></span>
4. <span data-ttu-id="8ef4b-116">Після того, як Outlook закривається, перезапустіть Outlook і повторіть кроки 2-3.</span><span class="sxs-lookup"><span data-stu-id="8ef4b-116">After Outlook closes, restart Outlook and repeat steps 2-3.</span></span> 
5. <span data-ttu-id="8ef4b-117">Після видалення вкладення натисніть кнопку **Надіслати/отримати** > **роботу автономно** , щоб скасувати вибір кнопки та відновити роботу в Інтернеті.</span><span class="sxs-lookup"><span data-stu-id="8ef4b-117">After you remove the attachment, click **Send / Receive** > **Work Offline** to deselect the button and to resume working online.</span></span> 

<span data-ttu-id="8ef4b-118">Повідомлення також застрягають в папці "Вихідні" після натискання кнопки " **Надіслати**", але ви не підключені.</span><span class="sxs-lookup"><span data-stu-id="8ef4b-118">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="8ef4b-119">Натисніть **Надіслати/отримати** та подивіться на кнопку **Автономна робота** .</span><span class="sxs-lookup"><span data-stu-id="8ef4b-119">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="8ef4b-120">Якщо це синій, ви відключені.</span><span class="sxs-lookup"><span data-stu-id="8ef4b-120">If it's blue, you're disconnected.</span></span> <span data-ttu-id="8ef4b-121">Натисніть його, щоб з'єднатися (кнопка стає білим) і натисніть кнопку **відправити все**.</span><span class="sxs-lookup"><span data-stu-id="8ef4b-121">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="8ef4b-122">**Увімкнути надсилання одразу після підключення**</span><span class="sxs-lookup"><span data-stu-id="8ef4b-122">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="8ef4b-123">На вкладці "файл" натисніть кнопку **"Параметри**".</span><span class="sxs-lookup"><span data-stu-id="8ef4b-123">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="8ef4b-124">У діалоговому вікні Параметри Outlook натисніть кнопку " **Додатково**".</span><span class="sxs-lookup"><span data-stu-id="8ef4b-124">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="8ef4b-125">У розділі надсилання й отримання клацніть, щоб увімкнути **надсилання одразу після підключення**.</span><span class="sxs-lookup"><span data-stu-id="8ef4b-125">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="8ef4b-126">Натисніть кнопку **OK**.</span><span class="sxs-lookup"><span data-stu-id="8ef4b-126">Click **OK**.</span></span>
 
<span data-ttu-id="8ef4b-127">Для отримання докладної інформації див.:</span><span class="sxs-lookup"><span data-stu-id="8ef4b-127">For full details, see:</span></span>
- [<span data-ttu-id="8ef4b-128">Відео: надсилання або видалення застрягли електронної пошти</span><span class="sxs-lookup"><span data-stu-id="8ef4b-128">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="8ef4b-129">Електронна пошта залишається в папці "Вихідні", доки вручну не ініціювати операцію надсилання й отримання в Outlook</span><span class="sxs-lookup"><span data-stu-id="8ef4b-129">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
