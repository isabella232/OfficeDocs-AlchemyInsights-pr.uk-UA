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
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959515"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="f0479-102">Outlook не вдалося підключитися до спільних папок</span><span class="sxs-lookup"><span data-stu-id="f0479-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="f0479-103">Якщо доступ до спільних папок не працює для кількох користувачів, спробуйте виконати наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="f0479-103">If public folder access isn't working for few users, try the following:</span></span>

<span data-ttu-id="f0479-104">Підключіться до EXO PowerShell і настройте DefaultPublicFolderMailbox на обліковий запис користувача, щоб відповідати один на робочий обліковий запис користувача.</span><span class="sxs-lookup"><span data-stu-id="f0479-104">Connect to EXO PowerShell, and configure the DefaultPublicFolderMailbox on the problem user account to match one on a working user account.</span></span>

<span data-ttu-id="f0479-105">Приклад:</span><span class="sxs-lookup"><span data-stu-id="f0479-105">Example:</span></span>

<span data-ttu-id="f0479-106">Отримати-поштову скриньку WorkingUser | DefaultPublicFolderMailbox FT, ефективність поштової скриньки</span><span class="sxs-lookup"><span data-stu-id="f0479-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="f0479-107">Проблеми з настроювання поштової скриньки-DefaultPublicFolderMailbox \<значення з попередньої команди></span><span class="sxs-lookup"><span data-stu-id="f0479-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="f0479-108">Зачекайте принаймні одну годину, щоб зміни набрали сили.</span><span class="sxs-lookup"><span data-stu-id="f0479-108">Wait at least one hour for the change to take effect.</span></span>