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
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930996"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="1b064-102">Служба Active Directory не синхронізується</span><span class="sxs-lookup"><span data-stu-id="1b064-102">Active Directory not syncing</span></span>

<span data-ttu-id="1b064-103">Якщо ви отримуєте помилки синхронізації, наприклад "нещодавня синхронізація" або помітили стан синхронізації служби каталогів на порталі адміністрування Office промовить фраза "Востаннє синхронізовано більше трьох днів тому", можливо, AADConnect має неправильні параметри або недостатньо дозволів на синхронізацію.</span><span class="sxs-lookup"><span data-stu-id="1b064-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="1b064-104">Якщо повторно інсталювати AADConnect за допомогою швидких настройок, проблему можна швидко вирішити.</span><span class="sxs-lookup"><span data-stu-id="1b064-104">Reinstalling AADConnect by using express settings might resolve the issue quickly:</span></span>

1. <span data-ttu-id="1b064-105">[Завантажте найновішу версію AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="1b064-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="1b064-106">[Дотримуйтеся вказівок щодо швидкого інсталяції](/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="1b064-106">[Follow the instructions for express installation](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="1b064-107">У Windows Server 2012 або пізніших версіях має бути інстальовано Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="1b064-107">Azure AD Connect must be installed on Windows Server 2012 or later.</span></span> <span data-ttu-id="1b064-108">Цей сервер має бути підключений до домену та може бути контролером домену або сервером-учасником.</span><span class="sxs-lookup"><span data-stu-id="1b064-108">This server must be domain joined and may be a domain controller or a member server.</span></span> <span data-ttu-id="1b064-109">Повний список вимог і попередніх Підключення Azure AD див. в передумови [для Azure AD Підключення](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span><span class="sxs-lookup"><span data-stu-id="1b064-109">For a full list of Azure AD Connect requirements and pre-requisites, review [Prerequisites for Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span></span>

<span data-ttu-id="1b064-110">Докладні відомості про облікові записи служб AADConnect див. в розділі [Azure AD Підключення: облікові записи та дозволи.](/azure/active-directory/hybrid/reference-connect-accounts-permissions)</span><span class="sxs-lookup"><span data-stu-id="1b064-110">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
