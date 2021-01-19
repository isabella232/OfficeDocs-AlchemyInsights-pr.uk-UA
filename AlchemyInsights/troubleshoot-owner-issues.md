---
title: Усунення проблем із власником
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7815"
- "9004358"
ms.openlocfilehash: 914d5682a403197a8569bb75fda8a77449f485f6
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901273"
---
# <a name="troubleshoot-owner-issues"></a><span data-ttu-id="8ceed-102">Усунення проблем із власником</span><span class="sxs-lookup"><span data-stu-id="8ceed-102">Troubleshoot owner issues</span></span>

<span data-ttu-id="8ceed-103">Щоб усунути проблеми, пов'язані з власником, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="8ceed-103">To troubleshoot owner-related issues, perform the following steps:</span></span>

1. <span data-ttu-id="8ceed-104">[Додавання або змінення адміністраторів "Лазурний](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners)": групи "блакитні активні каталоги" (AZURE AD) належать власникам груп і керуються ними.</span><span class="sxs-lookup"><span data-stu-id="8ceed-104">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): Azure Active Directory (Azure AD) groups are owned and managed by group owners.</span></span> <span data-ttu-id="8ceed-105">Власники групи можуть бути користувачами або службами, а також керувати групою, включно з членством.</span><span class="sxs-lookup"><span data-stu-id="8ceed-105">Group owners can be users or service principals, and are able to manage the group, including membership.</span></span> <span data-ttu-id="8ceed-106">Власникам групи можна призначати лише ті власники груп, а також керувати адміністраторами групи.</span><span class="sxs-lookup"><span data-stu-id="8ceed-106">Only existing group owners or group-managing administrators can assign group owners.</span></span> <span data-ttu-id="8ceed-107">Власники груп не повинні бути учасниками групи.</span><span class="sxs-lookup"><span data-stu-id="8ceed-107">Group owners aren't required to be members of the group.</span></span>
2. <span data-ttu-id="8ceed-108">[Додавання або змінення адміністраторів "Лазурний](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)": у цій статті описано, як додати або змінити роль адміністратора для користувача за допомогою azrbac в області "Передплата".</span><span class="sxs-lookup"><span data-stu-id="8ceed-108">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): This article describes how to add or change the administrator role for a user using Azure RBAC at the subscription scope.</span></span>
3. <span data-ttu-id="8ceed-109">Додайте власника групи або власника застосунку за допомогою PowerShell.</span><span class="sxs-lookup"><span data-stu-id="8ceed-109">Use PowerShell to add a group owner or an application owner.</span></span>
