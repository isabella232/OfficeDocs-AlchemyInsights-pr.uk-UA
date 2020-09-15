---
title: Служба Active Directory не синхронізується
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697650"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="0f883-102">Служба Active Directory не синхронізується</span><span class="sxs-lookup"><span data-stu-id="0f883-102">Active Directory not syncing</span></span>

<span data-ttu-id="0f883-103">Якщо ви отримуєте помилки синхронізації, наприклад "без нещодавньої синхронізації", або зверніть увагу на стан синхронізації служби каталогів на порталі адміністрування Office, говориться: "Востаннє синхронізовано більше 3 днів тому", можливо, це означає, що AADConnect має неправильні настройки або недостатні дозволи для виконання синхронізації.</span><span class="sxs-lookup"><span data-stu-id="0f883-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="0f883-104">Повторна інсталяція AADConnect за допомогою функції Експрес-параметрів може швидко вирішити проблему:</span><span class="sxs-lookup"><span data-stu-id="0f883-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="0f883-105">[Завантажте найновішу версію AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="0f883-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="0f883-106">[Виконайте вказівки з інсталяції Експрес](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)-програми.</span><span class="sxs-lookup"><span data-stu-id="0f883-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="0f883-107">Щоб отримати докладніші відомості про облікові записи служби AADConnect, перегляньте статтю [Azure AD Connect: облікові записи та дозволи](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="0f883-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
