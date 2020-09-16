---
title: Виправлення помилки 0x8004de40 в службі OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745151"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="f4e08-102">Виправлення помилки 0x8004de40 в службі OneDrive</span><span class="sxs-lookup"><span data-stu-id="f4e08-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="f4e08-103">Якщо ви отримали помилку 0x8004de40 із OneDrive:</span><span class="sxs-lookup"><span data-stu-id="f4e08-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="f4e08-104">Перезавантажте комп'ютер із відповідним комп'ютером під час підключення до вашого домену.</span><span class="sxs-lookup"><span data-stu-id="f4e08-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="f4e08-105">Якщо перезавантаження не усунуло проблему, ви не приєднуєтеся до свого пристрою в полі Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f4e08-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="f4e08-106">**Зверніть увагу**: ви маєте бути в корпоративній мережі, виконавши наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="f4e08-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="f4e08-107">Не робіть ці кроки, якщо ви не зможете підключитися до корпоративної інфраструктури (наприклад, під час подорожі).</span><span class="sxs-lookup"><span data-stu-id="f4e08-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="f4e08-108">Відкрийте командний рядок підвищеної якості.</span><span class="sxs-lookup"><span data-stu-id="f4e08-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="f4e08-109">Щоб відкрити командний рядок, натисніть кнопку **Пуск**, клацніть правою кнопкою миші пункт **командний рядок**і виберіть пункт **Запуск із правами адміністратора**.</span><span class="sxs-lookup"><span data-stu-id="f4e08-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="f4e08-110">Введіть *dsregcmd/Leave* і натисніть клавішу **ввід**.</span><span class="sxs-lookup"><span data-stu-id="f4e08-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="f4e08-111">Після завершення введіть *dsregcmd/JOIN* і натисніть клавішу **ввід**.</span><span class="sxs-lookup"><span data-stu-id="f4e08-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="f4e08-112">Після завершення закрийте командний рядок.</span><span class="sxs-lookup"><span data-stu-id="f4e08-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="f4e08-113">Перезавантажте комп'ютер і увійдіть у службу "OneDrive".</span><span class="sxs-lookup"><span data-stu-id="f4e08-113">Reboot the computer, and log into OneDrive.</span></span>