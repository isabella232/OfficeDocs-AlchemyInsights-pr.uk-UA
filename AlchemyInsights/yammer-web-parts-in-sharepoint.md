---
title: Веб-частини Yammer в SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5475"
- "9002494"
ms.openlocfilehash: 6868d7cdbbcc7d73e7e65fa0b0c954b4cba619ff
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198386"
---
# <a name="yammer-web-parts-in-sharepoint"></a><span data-ttu-id="0ef63-102">Веб-частини Yammer в SharePoint</span><span class="sxs-lookup"><span data-stu-id="0ef63-102">Yammer web parts in SharePoint</span></span>

<span data-ttu-id="0ef63-103">Бесіди Yammer та Yammer веб-частини мають покращити співпрацю на сучасних та класичних сторінках SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0ef63-103">Yammer Conversations and Yammer Highlights web parts enhance collaboration on modern and classic SharePoint pages.</span></span> <span data-ttu-id="0ef63-104">Для отримання додаткових [відомостей див.](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#conversations) [Yammer Highlights](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#highlights)</span><span class="sxs-lookup"><span data-stu-id="0ef63-104">For more info, see [Yammer Conversations](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#conversations)  and  [Yammer Highlights](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#highlights).</span></span>    

<span data-ttu-id="0ef63-105">Сучасні сеанси Yammer, веб-частина оновлюється новий досвід Yammer і доступний для цільових випуск орендарів.</span><span class="sxs-lookup"><span data-stu-id="0ef63-105">The modern Yammer Conversations web part is being updated to the new Yammer experience and is available for Targeted Release tenants.</span></span> <span data-ttu-id="0ef63-106">Початок впровадження GA.</span><span class="sxs-lookup"><span data-stu-id="0ef63-106">GA rollout has started.</span></span> <span data-ttu-id="0ef63-107">Нові можливості включають можливість почати розмову з будь-яким пост (питання, опитування, Хвала) і позначати найкращі відповіді безпосередньо з SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0ef63-107">New features include the ability to start a conversation with any post (Questions, Polls, Praise) and to mark best answers directly from SharePoint.</span></span> <span data-ttu-id="0ef63-108">Додаткові відомості наведено в розділі [нові умови клієнта Yammer та поширені запитання](https://docs.microsoft.com/yammer/get-started-with-yammer/newyammer-faq).</span><span class="sxs-lookup"><span data-stu-id="0ef63-108">For more info, see [New Yammer customer terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/newyammer-faq).</span></span>

 <span data-ttu-id="0ef63-109">Щоб зрозуміти, яка веб-частина та конфігурація є правильним для вас, перегляньте [використання веб-частини Yammer в SharePoint Online](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da).</span><span class="sxs-lookup"><span data-stu-id="0ef63-109">To understand which web part and configuration is right for you, see [Use a Yammer web part in SharePoint Online](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da).</span></span>  

<span data-ttu-id="0ef63-110">**Використання веб-частин із сервером SharePoint**</span><span class="sxs-lookup"><span data-stu-id="0ef63-110">**Using web parts with SharePoint Server**</span></span>  

<span data-ttu-id="0ef63-111">Веб-частини можна використовувати в сучасних і класичних сторінках в локальних середовищах.</span><span class="sxs-lookup"><span data-stu-id="0ef63-111">Web parts can be used in modern and classic pages within on-premises environments.</span></span>

- <span data-ttu-id="0ef63-112">Щоб отримати додаткові відомості про сучасні сторінки, див. [Додавання Фіду Yammer на сучасну сторінку в SharePoint Server 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-modern-page-in-sharepoint-server-2019).</span><span class="sxs-lookup"><span data-stu-id="0ef63-112">For more info about modern pages, see [Add a Yammer feed to a modern page in SharePoint Server 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-modern-page-in-sharepoint-server-2019).</span></span> 
- <span data-ttu-id="0ef63-113">Додаткові відомості про класичні сторінки див. [Додавання Фіду Yammer до класичної сторінки на серверах SharePoint 2013, 2016 та 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-classic-page-in-sharepoint-servers-2013-2016-and-2019).</span><span class="sxs-lookup"><span data-stu-id="0ef63-113">For more info about classic pages, see [Add a Yammer feed to a classic page in SharePoint Servers 2013, 2016, and 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-classic-page-in-sharepoint-servers-2013-2016-and-2019).</span></span>

<span data-ttu-id="0ef63-114">**Вбудувати Yammer**</span><span class="sxs-lookup"><span data-stu-id="0ef63-114">**Yammer Embed**</span></span>  

<span data-ttu-id="0ef63-115">Скористайтеся інструментом "Вбудувати конфігурацію" для перевірки використання вбудовування.</span><span class="sxs-lookup"><span data-stu-id="0ef63-115">Use the Embed Configuration tool to test Embed usage.</span></span> <span data-ttu-id="0ef63-116">Майбутні оновлення для впровадження дасть змогу новий досвід Yammer.</span><span class="sxs-lookup"><span data-stu-id="0ef63-116">A future update to Embed will enable the new Yammer experience.</span></span> <span data-ttu-id="0ef63-117">Щоб дізнатися більше, зверніться до [засобу настроювання Yammer](https://aka.ms/YammerEmbedConfigureTool).</span><span class="sxs-lookup"><span data-stu-id="0ef63-117">For more info, see the [Yammer Embed Configuration tool](https://aka.ms/YammerEmbedConfigureTool).</span></span> <span data-ttu-id="0ef63-118">Щоб краще зрозуміти [компонент вбудування Yammer, див.](https://aka.ms/YammerDevDocs)</span><span class="sxs-lookup"><span data-stu-id="0ef63-118">To better understand the Yammer Embed component, see [Embed Feed](https://aka.ms/YammerDevDocs).</span></span>

<span data-ttu-id="0ef63-119">**Відомі проблеми та обмеження**</span><span class="sxs-lookup"><span data-stu-id="0ef63-119">**Known issues and limitations**</span></span>

- <span data-ttu-id="0ef63-120">Ідентифікатори групи недоступні з нових URL-адрес Yammer, які змінилися.</span><span class="sxs-lookup"><span data-stu-id="0ef63-120">Group IDs are not available from new Yammer URLs, which have changed.</span></span> <span data-ttu-id="0ef63-121">Поверніться до класичного режиму, щоб отримати ідентифікатори групи або інші ідентифікатори з URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="0ef63-121">Switch back to classic mode to obtain group IDs or other IDs from URLs.</span></span>
- <span data-ttu-id="0ef63-122">Настроювані (марнославства) домени не підтримуються.</span><span class="sxs-lookup"><span data-stu-id="0ef63-122">Custom (vanity) domains are not supported.</span></span>
- <span data-ttu-id="0ef63-123">Вставляти Yammer не оптимізовано для мобільних пристроїв.</span><span class="sxs-lookup"><span data-stu-id="0ef63-123">Yammer Embed is not optimized for mobile.</span></span> <span data-ttu-id="0ef63-124">Використовуйте сучасні сторінки з веб-частиною «бесіди Yammer» для кращої роботи.</span><span class="sxs-lookup"><span data-stu-id="0ef63-124">Use modern pages with the Yammer Conversations web part for the best experience.</span></span>
- <span data-ttu-id="0ef63-125">Настроювані теми, можуть впливати на зовнішній вигляд і зручність використання веб-частина Yammer розмов.</span><span class="sxs-lookup"><span data-stu-id="0ef63-125">Custom themes can affect the appearance and usability of the Yammer Conversations web part.</span></span> <span data-ttu-id="0ef63-126">Відкрийте інцидент підтримки, щоб повідомити про проблеми.</span><span class="sxs-lookup"><span data-stu-id="0ef63-126">Open a support case to report issues.</span></span>