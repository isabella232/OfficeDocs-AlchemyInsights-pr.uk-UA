---
title: Служба Active Directory не синхронізується
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822872"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="df868-102">Служба Active Directory не синхронізується</span><span class="sxs-lookup"><span data-stu-id="df868-102">Active Directory not syncing</span></span>

<span data-ttu-id="df868-103">Якщо ви отримуєте помилки синхронізації, наприклад "нещодавня синхронізація" або помітили стан синхронізації служби каталогів на порталі адміністрування Office, промовляється "Востаннє синхронізовано більше трьох днів тому", можливо, AADConnect має неправильні параметри або недостатньо дозволів на синхронізацію.</span><span class="sxs-lookup"><span data-stu-id="df868-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="df868-104">Якщо повторно інсталювати AADConnect за допомогою швидких настройок, проблему можна швидко вирішити.</span><span class="sxs-lookup"><span data-stu-id="df868-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="df868-105">[Завантажте найновішу версію AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="df868-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="df868-106">[Дотримуйтеся вказівок щодо швидкого інсталяції](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="df868-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="df868-107">Докладні відомості про облікові записи служб AADConnect див. в розділі [Azure AD Connect: облікові записи та дозволи.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)</span><span class="sxs-lookup"><span data-stu-id="df868-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
