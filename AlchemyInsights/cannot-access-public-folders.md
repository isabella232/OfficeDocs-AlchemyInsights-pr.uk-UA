---
title: Не вдається отримати доступ до спільних папок
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891770"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="df0e0-102">Outlook не вдалося підключитися до спільних папок</span><span class="sxs-lookup"><span data-stu-id="df0e0-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="df0e0-103">Якщо доступ до спільних папок не працює для деяких користувачів, спробуйте виконати наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="df0e0-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="df0e0-104">Підключіться до EXO PowerShell і настройте параметр DefaultPublicFolderMailbox на обліковий запис користувача, щоб зіставити параметр у робочий обліковий запис користувача.</span><span class="sxs-lookup"><span data-stu-id="df0e0-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="df0e0-105">Приклад:</span><span class="sxs-lookup"><span data-stu-id="df0e0-105">Example:</span></span>

<span data-ttu-id="df0e0-106">Отримати-поштову скриньку WorkingUser | DefaultPublicFolderMailbox FT, ефективність поштової скриньки</span><span class="sxs-lookup"><span data-stu-id="df0e0-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="df0e0-107">Проблеми з настроювання поштової скриньки-DefaultPublicFolderMailbox \<значення з попередньої команди></span><span class="sxs-lookup"><span data-stu-id="df0e0-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="df0e0-108">Зачекайте принаймні одну годину, щоб зміни набрали сили.</span><span class="sxs-lookup"><span data-stu-id="df0e0-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="df0e0-109">Якщо проблема залишається, будь ласка, дотримуйтесь [цієї процедури](https://aka.ms/pfcte) для усунення проблем із доступом до спільних папок, використовуючи Outlook.</span><span class="sxs-lookup"><span data-stu-id="df0e0-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>