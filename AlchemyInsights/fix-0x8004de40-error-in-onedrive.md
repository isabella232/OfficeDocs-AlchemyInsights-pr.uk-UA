---
title: Виправлено помилку 0x8004de40 у OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: aa0e0a63ac1e365a7cdce018626740446040a664
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755869"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="8fed5-102">Виправлено помилку 0x8004de40 у OneDrive</span><span class="sxs-lookup"><span data-stu-id="8fed5-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="8fed5-103">Якщо помилка 0x8004de40 з OneDrive:</span><span class="sxs-lookup"><span data-stu-id="8fed5-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="8fed5-104">Перезавантажте комп'ютер, що впливає під час підключення до домену Acitve каталогу.</span><span class="sxs-lookup"><span data-stu-id="8fed5-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="8fed5-105">Якщо перезавантаження не виправити проблему, unjoin і повторно приєднатися до пристрою з Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8fed5-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="8fed5-106">**Зверніть увагу**: ви повинні бути в корпоративній мережі під час виконання цих дій.</span><span class="sxs-lookup"><span data-stu-id="8fed5-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="8fed5-107">Не виконуйте ці дії, якщо не вдається підключитися до корпоративної інфраструктури (наприклад, під час подорожі).</span><span class="sxs-lookup"><span data-stu-id="8fed5-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="8fed5-108">Відкрийте командний рядок у режимі адміністратора.</span><span class="sxs-lookup"><span data-stu-id="8fed5-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="8fed5-109">Щоб відкрити командний рядок у режимі адміністратора, натисніть кнопку **Пуск**, клацніть правою кнопкою миші пункт Командний **рядок**і виберіть пункт Запуск із правами **адміністратора**.</span><span class="sxs-lookup"><span data-stu-id="8fed5-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="8fed5-110">Введіть *dmregcmd/залишити* і натисніть клавішу **Enter**.</span><span class="sxs-lookup"><span data-stu-id="8fed5-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="8fed5-111">Після завершення введіть *ddregcmd/JOIN* і натисніть клавішу **Enter**.</span><span class="sxs-lookup"><span data-stu-id="8fed5-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="8fed5-112">Після завершення, закрийте командний рядок.</span><span class="sxs-lookup"><span data-stu-id="8fed5-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="8fed5-113">Перезавантажте комп'ютер і ввійдіть до OneDrive.</span><span class="sxs-lookup"><span data-stu-id="8fed5-113">Reboot the computer, and log into OneDrive.</span></span>