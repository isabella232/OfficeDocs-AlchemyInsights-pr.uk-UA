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
ms.openlocfilehash: d436184bdc0e283db217ea734fb2c8e05f85b4e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525080"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="22ec3-102">Виправити помилку 0x8004de40 в OneDrive</span><span class="sxs-lookup"><span data-stu-id="22ec3-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="22ec3-103">Якщо ви отримали повідомлення про помилку 0x8004de40 з OneDrive:</span><span class="sxs-lookup"><span data-stu-id="22ec3-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="22ec3-104">Перезавантаження постраждалих комп'ютера при підключенні до вашого домену активний Directory.</span><span class="sxs-lookup"><span data-stu-id="22ec3-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="22ec3-105">Якщо перезавантаження системи не вирішити проблему, видалення і возз'єднатися вашого пристрою з блакитні оголошення.</span><span class="sxs-lookup"><span data-stu-id="22ec3-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="22ec3-106">**Примітка**: ви повинні бути корпоративної мережі під час виконання цих дій.</span><span class="sxs-lookup"><span data-stu-id="22ec3-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="22ec3-107">Не виконувати ці дії, коли вам не вдається підключитися до корпоративної інфраструктури (наприклад, під час подорожі).</span><span class="sxs-lookup"><span data-stu-id="22ec3-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="22ec3-108">Відкрити підвищеної командного рядка.</span><span class="sxs-lookup"><span data-stu-id="22ec3-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="22ec3-109">Відкрити підвищеної командного рядка, клацніть - **почати**, клацніть правою кнопкою миші **командний рядок**і виберіть пункт **Запуск із правами адміністратора**.</span><span class="sxs-lookup"><span data-stu-id="22ec3-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="22ec3-110">Введіть *dsregcmd /leave* і натисніть клавішу **Enter**.</span><span class="sxs-lookup"><span data-stu-id="22ec3-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="22ec3-111">Завершеним, введіть *dsregcmd /join* і натисніть клавішу **Enter**.</span><span class="sxs-lookup"><span data-stu-id="22ec3-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="22ec3-112">Завершеним, Закрийте вікно командного рядка.</span><span class="sxs-lookup"><span data-stu-id="22ec3-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="22ec3-113">Перезавантажити комп'ютер і ввійти в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="22ec3-113">Reboot the computer, and log into OneDrive.</span></span>