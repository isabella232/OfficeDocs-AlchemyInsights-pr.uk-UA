---
title: Active Directory не синхронізується
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265277"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="92975-102">Active Directory не синхронізується</span><span class="sxs-lookup"><span data-stu-id="92975-102">Active Directory not syncing</span></span>

<span data-ttu-id="92975-103">Якщо ви отримуєте помилки синхронізації, наприклад, "немає останньої синхронізації" або зверніть увагу на стан синхронізації каталогів на порталі Office Admin говориться, "Остання синхронізація більше 3 днів тому", може бути, що AADConnect має неправильні параметри або недостатньо дозволи на виконання синхронізації.</span><span class="sxs-lookup"><span data-stu-id="92975-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="92975-104">Повторна інсталяція AADConnect за допомогою Експрес-настройок може швидко вирішити проблему:</span><span class="sxs-lookup"><span data-stu-id="92975-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="92975-105">[Завантажити останню версію AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="92975-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="92975-106">[Дотримуйтеся вказівок для Експрес-інсталяції](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="92975-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="92975-107">Щоб отримати додаткові відомості про AADConnect служби облікових записів, див [AZURE AD-підключення: облікові записи та дозволи](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="92975-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
