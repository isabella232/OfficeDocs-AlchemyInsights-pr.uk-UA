---
title: Виправлено помилку 0x8004de40 у OneDrive
ms.author: pebaum
author: pebaum
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 48b29f57763ca22a71a23b2afddcac0e8e8a95db
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052058"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="d9ba6-102">Виправлено помилку 0x8004de40 у OneDrive</span><span class="sxs-lookup"><span data-stu-id="d9ba6-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="d9ba6-103">Якщо помилка 0x8004de40 з OneDrive:</span><span class="sxs-lookup"><span data-stu-id="d9ba6-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="d9ba6-104">Перезавантажте комп'ютер, що впливає під час підключення до домену Acitve каталогу.</span><span class="sxs-lookup"><span data-stu-id="d9ba6-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="d9ba6-105">Якщо перезавантаження не виправити проблему, unjoin і повторно приєднатися до пристрою з Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d9ba6-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="d9ba6-106">**Зверніть увагу**: ви повинні бути в корпоративній мережі під час виконання цих дій.</span><span class="sxs-lookup"><span data-stu-id="d9ba6-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="d9ba6-107">Не виконуйте ці дії, якщо не вдається підключитися до корпоративної інфраструктури (наприклад, під час подорожі).</span><span class="sxs-lookup"><span data-stu-id="d9ba6-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="d9ba6-108">Відкрийте командний рядок у режимі адміністратора.</span><span class="sxs-lookup"><span data-stu-id="d9ba6-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="d9ba6-109">Щоб відкрити командний рядок у режимі адміністратора, натисніть кнопку **Пуск**, клацніть правою кнопкою миші пункт Командний **рядок**і виберіть пункт Запуск із правами **адміністратора**.</span><span class="sxs-lookup"><span data-stu-id="d9ba6-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="d9ba6-110">Введіть *dmregcmd/залишити* і натисніть клавішу **Enter**.</span><span class="sxs-lookup"><span data-stu-id="d9ba6-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="d9ba6-111">Після завершення введіть *ddregcmd/JOIN* і натисніть клавішу **Enter**.</span><span class="sxs-lookup"><span data-stu-id="d9ba6-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="d9ba6-112">Після завершення, закрийте командний рядок.</span><span class="sxs-lookup"><span data-stu-id="d9ba6-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="d9ba6-113">Перезавантажте комп'ютер і ввійдіть до OneDrive.</span><span class="sxs-lookup"><span data-stu-id="d9ba6-113">Reboot the computer, and log into OneDrive.</span></span>