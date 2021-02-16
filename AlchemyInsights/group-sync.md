---
title: Синхронізація групи
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8304"
- "9003234"
ms.openlocfilehash: 52c19b6dcc79968150a188b389c5481c122f7945
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256913"
---
# <a name="group-sync"></a><span data-ttu-id="7b280-102">Синхронізація групи</span><span class="sxs-lookup"><span data-stu-id="7b280-102">Group sync</span></span>

<span data-ttu-id="7b280-103">У цій статті наведено вказівки щодо синхронізації групи.</span><span class="sxs-lookup"><span data-stu-id="7b280-103">This article provides guidance on group synchronization.</span></span>

1. <span data-ttu-id="7b280-104">Якщо Глобальний адміністратор або власник групи не зможе змінити властивості групи або додати учасників або призначити власників на порталі лазур, переконайтеся, що джерело повноважень групи – «Лазурний» («Лазурний») для глобального адміністратора або власника групи, щоб змінити групу.</span><span class="sxs-lookup"><span data-stu-id="7b280-104">If a global admin or group owner is not able to modify group properties or add members or assign owners in the Azure portal, ensure the source of the authority for the group is Azure Active Directory (Azure AD) for the global admin or group owner to modify the group.</span></span>
2. <span data-ttu-id="7b280-105">Перш ніж видалити синхронізовану групу в Azure AD, переконайтеся, що ви [видалили всі призначені ліцензії](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) , щоб уникнути помилок.</span><span class="sxs-lookup"><span data-stu-id="7b280-105">Before attempting to delete a synced group in Azure AD, ensure you have [deleted all assigned licenses](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) to avoid errors.</span></span>

<span data-ttu-id="7b280-106">Щоб дізнатися, як синхронізувати користувачів, групи та контакти, ознайомтеся з [синхронізацією служби AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts), а [потім синхронізуйте локальну групу за допомогою служби Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) , щоб синхронізувати в-ПЕРМНІ групи за допомогою AD Connect.</span><span class="sxs-lookup"><span data-stu-id="7b280-106">For understanding how to sync users, groups and contacts, see [Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts), and follow [Syncing an on-premises group to Azure using Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) to sync on-perm groups using AD connect.</span></span>

<span data-ttu-id="7b280-107">Під час синхронізації дотримуйтеся [помилок виправлення неполадок](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) , щоб усунути поширені помилки під час синхронізації.</span><span class="sxs-lookup"><span data-stu-id="7b280-107">Follow this guide [Troubleshooting Errors during synchronization](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) to troubleshoot common errors during synchronization.</span></span>

