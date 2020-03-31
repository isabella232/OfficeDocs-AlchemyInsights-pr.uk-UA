---
title: Змінення дозволів для спільної папки
ms.author: dmaguire
author: msdmaguire
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "633"
- "3500007"
ms.assetid: 0c37ab75-c81c-44e7-bda8-ea43263f9fdf
ms.openlocfilehash: 68aefd820c681a9022828f67655e1c843692a30e
ms.sourcegitcommit: 92e9a649532f5231ceedcafc4d14b8ad18d517c2
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/31/2020
ms.locfileid: "43059793"
---
# <a name="changing-public-folder-permissions"></a><span data-ttu-id="9eef0-102">Змінення дозволів для спільної папки</span><span class="sxs-lookup"><span data-stu-id="9eef0-102">Changing public folder permissions</span></span>

<span data-ttu-id="9eef0-103">Дозволи для спільної папки можуть бути змінені користувачами та адміністраторами в Outlook.</span><span class="sxs-lookup"><span data-stu-id="9eef0-103">Public folder permissions can be changed by users and administrators in Outlook.</span></span> <span data-ttu-id="9eef0-104">Адміністратори також можуть керувати дозволами від центру адміністрування Exchange (EАС), виконавши такі дії:</span><span class="sxs-lookup"><span data-stu-id="9eef0-104">Administrators can also control permissions from the Exchange Admin Center (EAC), by doing the following:</span></span>
  
1. <span data-ttu-id="9eef0-105">У Microsoft 365 Центр адміністрування, перейдіть до **адміністратора центри** \> **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="9eef0-105">In the Microsoft 365 admin center, go to **Admin centers** \> **Exchange**.</span></span>

2. <span data-ttu-id="9eef0-106">Виберіть **спільних папок**.</span><span class="sxs-lookup"><span data-stu-id="9eef0-106">Select **Public folders**.</span></span>

3. <span data-ttu-id="9eef0-107">Звідти можна змінити дозволи для окремих спільних папок, призначивши групи безпеки для дозволів.</span><span class="sxs-lookup"><span data-stu-id="9eef0-107">From there, you can change permissions for individual public folders by assigning security groups to permissions.</span></span> <span data-ttu-id="9eef0-108">Для кінцевого користувача, щоб змінити дозволи на доступ до спільних папок, користувач має права власника в папці.</span><span class="sxs-lookup"><span data-stu-id="9eef0-108">For an end user to change public folder permissions, the user needs to have Owner rights on the folder.</span></span>

<span data-ttu-id="9eef0-109">Будь ласка, дотримуйтесь процедури, описаної в [як діагностувати та виправити спільних папок дозволів проблеми](https://docs.microsoft.com/exchange/troubleshoot/public-folders/public-folder-permission-issues) для виправлення неполадок спільних папок.</span><span class="sxs-lookup"><span data-stu-id="9eef0-109">Please follow the procedure described in [How to diagnose and fix public folder permission issues](https://docs.microsoft.com/exchange/troubleshoot/public-folders/public-folder-permission-issues) to troubleshoot public folder permission issues.</span></span>

<span data-ttu-id="9eef0-110">**Примітка**: є кілька відомих проблем, які можуть виникнути під час спроби змінити дозволи на доступ до спільних папок.</span><span class="sxs-lookup"><span data-stu-id="9eef0-110">**Note**: There are several known issues you might encounter when you try to change permissions on public folders.</span></span> <span data-ttu-id="9eef0-111">Щоб отримати додаткові відомості, перегляньте наведені нижче статті.</span><span class="sxs-lookup"><span data-stu-id="9eef0-111">See the following articles for more information.</span></span>

- [<span data-ttu-id="9eef0-112">Не вдається застосувати дозволи на спільних папок вкладені папки на рівні</span><span class="sxs-lookup"><span data-stu-id="9eef0-112">Can't apply permissions to public folder subfolders in EAC</span></span>](https://docs.microsoft.com/exchange/troubleshoot/public-folders/can%E2%80%99t-apply-permissions-public-folder-subfolders)

- [<span data-ttu-id="9eef0-113">"Поштову скриньку не знайдено в локальному лісі" помилка під час доступу до спільних папок</span><span class="sxs-lookup"><span data-stu-id="9eef0-113">"The mailbox is not found in the local forest" error when you access public folders</span></span>](https://docs.microsoft.com/exchange/troubleshoot/public-folders/mailbox-not-found-local-forest-public-folder)
