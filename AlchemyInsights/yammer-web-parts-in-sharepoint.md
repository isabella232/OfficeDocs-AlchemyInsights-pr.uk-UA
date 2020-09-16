---
title: Веб-частини Yammer на сайті SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5475"
- "9002494"
ms.openlocfilehash: d8b4043bb2889429a18c477505e7eca662943051
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664371"
---
# <a name="yammer-web-parts-in-sharepoint"></a><span data-ttu-id="44bc7-102">Веб-частини Yammer на сайті SharePoint</span><span class="sxs-lookup"><span data-stu-id="44bc7-102">Yammer web parts in SharePoint</span></span>

<span data-ttu-id="44bc7-103">Розмови Yammer і Yammer виділяє веб-частини, які підвищують співпрацю на сучасних і класичних сторінках SharePoint.</span><span class="sxs-lookup"><span data-stu-id="44bc7-103">Yammer Conversations and Yammer Highlights web parts enhance collaboration on modern and classic SharePoint pages.</span></span> <span data-ttu-id="44bc7-104">Докладні відомості наведено в статті " [розмови Yammer](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#conversations)  " та "  [Yammer](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#highlights)".</span><span class="sxs-lookup"><span data-stu-id="44bc7-104">For more info, see [Yammer Conversations](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#conversations)  and  [Yammer Highlights](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#highlights).</span></span>    

<span data-ttu-id="44bc7-105">Сучасна веб-частина "розмови Yammer" оновлюється в новому досвіді Yammer та доступна для клієнтів цільового випуску.</span><span class="sxs-lookup"><span data-stu-id="44bc7-105">The modern Yammer Conversations web part is being updated to the new Yammer experience and is available for Targeted Release tenants.</span></span> <span data-ttu-id="44bc7-106">Початок роботи з GA.</span><span class="sxs-lookup"><span data-stu-id="44bc7-106">GA rollout has started.</span></span> <span data-ttu-id="44bc7-107">Нові функції включають можливість почати розмову з будь-якими публічниками (питаннями, опитуваннями, похвалами), а також позначатися відповіді на них безпосередньо в службі SharePoint.</span><span class="sxs-lookup"><span data-stu-id="44bc7-107">New features include the ability to start a conversation with any post (Questions, Polls, Praise) and to mark best answers directly from SharePoint.</span></span> <span data-ttu-id="44bc7-108">Щоб отримати докладні відомості, ознайомтеся з [новими умовами клієнта Yammer та відповіді](https://docs.microsoft.com/yammer/get-started-with-yammer/newyammer-faq)на них.</span><span class="sxs-lookup"><span data-stu-id="44bc7-108">For more info, see [New Yammer customer terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/newyammer-faq).</span></span>

 <span data-ttu-id="44bc7-109">Щоб зрозуміти, яка веб-частина та конфігурація вам підходить, ознайомтеся з [веб-частиною Yammer у службі SharePoint Online](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da).</span><span class="sxs-lookup"><span data-stu-id="44bc7-109">To understand which web part and configuration is right for you, see [Use a Yammer web part in SharePoint Online](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da).</span></span>  

<span data-ttu-id="44bc7-110">**Використання веб-частин із сервером SharePoint Server**</span><span class="sxs-lookup"><span data-stu-id="44bc7-110">**Using web parts with SharePoint Server**</span></span>  

<span data-ttu-id="44bc7-111">Веб-частини можна використовувати в сучасних і класичних сторінках в локальних середовищах.</span><span class="sxs-lookup"><span data-stu-id="44bc7-111">Web parts can be used in modern and classic pages within on-premises environments.</span></span>

- <span data-ttu-id="44bc7-112">Докладні відомості про сучасні сторінки наведено в статті [Додавання каналу Yammer до сучасної сторінки на сервері SharePoint Server 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-modern-page-in-sharepoint-server-2019).</span><span class="sxs-lookup"><span data-stu-id="44bc7-112">For more info about modern pages, see [Add a Yammer feed to a modern page in SharePoint Server 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-modern-page-in-sharepoint-server-2019).</span></span> 
- <span data-ttu-id="44bc7-113">Докладні відомості про класичні сторінки наведено в статті [Додавання каналу Yammer до класичної сторінки на серверах SharePoint 2013, 2016 і 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-classic-page-in-sharepoint-servers-2013-2016-and-2019).</span><span class="sxs-lookup"><span data-stu-id="44bc7-113">For more info about classic pages, see [Add a Yammer feed to a classic page in SharePoint Servers 2013, 2016, and 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-classic-page-in-sharepoint-servers-2013-2016-and-2019).</span></span>

<span data-ttu-id="44bc7-114">**Вбудовування Yammer**</span><span class="sxs-lookup"><span data-stu-id="44bc7-114">**Yammer Embed**</span></span>  

<span data-ttu-id="44bc7-115">Скористайтеся засобом вбудовування конфігурації, щоб перевірити використання вбудовування.</span><span class="sxs-lookup"><span data-stu-id="44bc7-115">Use the Embed Configuration tool to test Embed usage.</span></span> <span data-ttu-id="44bc7-116">Подальше оновлення для вбудовування дасть змогу створити новий досвід Yammer.</span><span class="sxs-lookup"><span data-stu-id="44bc7-116">A future update to Embed will enable the new Yammer experience.</span></span> <span data-ttu-id="44bc7-117">Щоб отримати докладні відомості, ознайомтеся з [засобом настроювання служби вбудовування Yammer](https://aka.ms/YammerEmbedConfigureTool).</span><span class="sxs-lookup"><span data-stu-id="44bc7-117">For more info, see the [Yammer Embed Configuration tool](https://aka.ms/YammerEmbedConfigureTool).</span></span> <span data-ttu-id="44bc7-118">Щоб краще зрозуміти компонент вбудовування Yammer, ознайомтеся з елементом [вбудовування каналу](https://aka.ms/YammerDevDocs).</span><span class="sxs-lookup"><span data-stu-id="44bc7-118">To better understand the Yammer Embed component, see [Embed Feed](https://aka.ms/YammerDevDocs).</span></span>

<span data-ttu-id="44bc7-119">**Відомі проблеми та обмеження**</span><span class="sxs-lookup"><span data-stu-id="44bc7-119">**Known issues and limitations**</span></span>

- <span data-ttu-id="44bc7-120">Ідентифікатори групи недоступні з нових URL-адрес Yammer, які змінилися.</span><span class="sxs-lookup"><span data-stu-id="44bc7-120">Group IDs are not available from new Yammer URLs, which have changed.</span></span> <span data-ttu-id="44bc7-121">Поверніться до класичного режиму, щоб отримати ідентифікатори групи або інші ідентифікатори з URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="44bc7-121">Switch back to classic mode to obtain group IDs or other IDs from URLs.</span></span>
- <span data-ttu-id="44bc7-122">Користувальницькі домени (марнославство) не підтримуються.</span><span class="sxs-lookup"><span data-stu-id="44bc7-122">Custom (vanity) domains are not supported.</span></span>
- <span data-ttu-id="44bc7-123">Вбудовування Yammer не оптимізовано для мобільних пристроїв.</span><span class="sxs-lookup"><span data-stu-id="44bc7-123">Yammer Embed is not optimized for mobile.</span></span> <span data-ttu-id="44bc7-124">Використовуйте сучасні сторінки з веб-частиною "розмови Yammer", щоб отримати кращий досвід.</span><span class="sxs-lookup"><span data-stu-id="44bc7-124">Use modern pages with the Yammer Conversations web part for the best experience.</span></span>
- <span data-ttu-id="44bc7-125">Користувацькі теми можуть вплинути на оформлення та зручність використання веб-частини "розмови Yammer".</span><span class="sxs-lookup"><span data-stu-id="44bc7-125">Custom themes can affect the appearance and usability of the Yammer Conversations web part.</span></span> <span data-ttu-id="44bc7-126">Відкрийте інцидент підтримки, щоб повідомити про проблеми.</span><span class="sxs-lookup"><span data-stu-id="44bc7-126">Open a support case to report issues.</span></span>