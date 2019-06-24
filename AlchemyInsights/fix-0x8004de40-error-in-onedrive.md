---
title: Виправити помилку 0x8004de40 в OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133997"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="09b2f-102">Виправити помилку 0x8004de40 в OneDrive</span><span class="sxs-lookup"><span data-stu-id="09b2f-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="09b2f-103">Якщо ви отримали повідомлення про помилку 0x8004de40 з OneDrive:</span><span class="sxs-lookup"><span data-stu-id="09b2f-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="09b2f-104">Перезавантаження постраждалих комп'ютера при підключенні до вашого домену активний Directory.</span><span class="sxs-lookup"><span data-stu-id="09b2f-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="09b2f-105">Якщо перезавантаження системи не вирішити проблему, видалення і возз'єднатися вашого пристрою з блакитні оголошення.</span><span class="sxs-lookup"><span data-stu-id="09b2f-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="09b2f-106">**Примітка**: ви повинні бути корпоративної мережі під час виконання цих дій.</span><span class="sxs-lookup"><span data-stu-id="09b2f-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="09b2f-107">Не виконувати ці дії, коли вам не вдається підключитися до корпоративної інфраструктури (наприклад, під час подорожі).</span><span class="sxs-lookup"><span data-stu-id="09b2f-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="09b2f-108">Відкрити підвищеної командного рядка.</span><span class="sxs-lookup"><span data-stu-id="09b2f-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="09b2f-109">Відкрити підвищеної командного рядка, клацніть - **почати**, клацніть правою кнопкою миші **командний рядок**і виберіть пункт **Запуск із правами адміністратора**.</span><span class="sxs-lookup"><span data-stu-id="09b2f-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="09b2f-110">Введіть *dsregcmd /leave* і натисніть клавішу **Enter**.</span><span class="sxs-lookup"><span data-stu-id="09b2f-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="09b2f-111">Завершеним, введіть *dsregcmd /join* і натисніть клавішу **Enter**.</span><span class="sxs-lookup"><span data-stu-id="09b2f-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="09b2f-112">Завершеним, Закрийте вікно командного рядка.</span><span class="sxs-lookup"><span data-stu-id="09b2f-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="09b2f-113">Перезавантажити комп'ютер і ввійти в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="09b2f-113">Reboot the computer, and log into OneDrive.</span></span>