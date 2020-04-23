---
title: Виправлено помилку 0x8004de40 у OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716049"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="3f5dc-102">Виправлено помилку 0x8004de40 у OneDrive</span><span class="sxs-lookup"><span data-stu-id="3f5dc-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="3f5dc-103">Якщо помилка 0x8004de40 з OneDrive:</span><span class="sxs-lookup"><span data-stu-id="3f5dc-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="3f5dc-104">Перезавантажте комп'ютер, що впливає під час підключення до домену Acitve каталогу.</span><span class="sxs-lookup"><span data-stu-id="3f5dc-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="3f5dc-105">Якщо перезавантаження не виправити проблему, unjoin і повторно приєднатися до пристрою з Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3f5dc-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="3f5dc-106">**Зверніть увагу**: ви повинні бути в корпоративній мережі під час виконання цих дій.</span><span class="sxs-lookup"><span data-stu-id="3f5dc-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="3f5dc-107">Не виконуйте ці дії, якщо не вдається підключитися до корпоративної інфраструктури (наприклад, під час подорожі).</span><span class="sxs-lookup"><span data-stu-id="3f5dc-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="3f5dc-108">Відкрийте командний рядок у режимі адміністратора.</span><span class="sxs-lookup"><span data-stu-id="3f5dc-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="3f5dc-109">Щоб відкрити командний рядок у режимі адміністратора, натисніть кнопку **Пуск**, клацніть правою кнопкою миші пункт Командний **рядок**і виберіть пункт Запуск із правами **адміністратора**.</span><span class="sxs-lookup"><span data-stu-id="3f5dc-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="3f5dc-110">Введіть *dmregcmd/залишити* і натисніть клавішу **Enter**.</span><span class="sxs-lookup"><span data-stu-id="3f5dc-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="3f5dc-111">Після завершення введіть *ddregcmd/JOIN* і натисніть клавішу **Enter**.</span><span class="sxs-lookup"><span data-stu-id="3f5dc-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="3f5dc-112">Після завершення, закрийте командний рядок.</span><span class="sxs-lookup"><span data-stu-id="3f5dc-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="3f5dc-113">Перезавантажте комп'ютер і ввійдіть до OneDrive.</span><span class="sxs-lookup"><span data-stu-id="3f5dc-113">Reboot the computer, and log into OneDrive.</span></span>