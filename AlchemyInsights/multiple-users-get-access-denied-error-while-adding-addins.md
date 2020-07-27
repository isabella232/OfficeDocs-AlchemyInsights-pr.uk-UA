---
title: Кілька користувачів отримати доступ відмовлено помилка під час додавання надбудови в Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424179"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="2a3ee-102">Кілька користувачів отримати доступ відмовлено помилка під час додавання надбудови в Outlook</span><span class="sxs-lookup"><span data-stu-id="2a3ee-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="2a3ee-103">Можна вказати, які адміністратори в організації мають дозволи на інсталяцію та керування надбудовами для Outlook.</span><span class="sxs-lookup"><span data-stu-id="2a3ee-103">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook.</span></span> <span data-ttu-id="2a3ee-104">Також можна вказати, які користувачі в організації мають дозвіл на інсталяцію та керування надбудовами для власного використання.</span><span class="sxs-lookup"><span data-stu-id="2a3ee-104">You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="2a3ee-105">Докладніше, перегляньте відомості про [указання адміністраторів і користувачів, які можуть інсталювати надбудови Outlook і керувати ними](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="2a3ee-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="2a3ee-106">Щоб переконатися, що ви успішно призначені дозволи для користувача, замініть <Role Name> ім'я ролі, щоб перевірити і виконайте таку команду в Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="2a3ee-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="2a3ee-107">Get-Управліннярольова призначення-роль " <Role Name> "-geteffectiveusers</span><span class="sxs-lookup"><span data-stu-id="2a3ee-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="2a3ee-108">У цьому прикладі пояснюється, як перевірити, кому призначено дозволи на інсталяцію надбудов із магазину Office для організації.</span><span class="sxs-lookup"><span data-stu-id="2a3ee-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="2a3ee-109">Powershell</span><span class="sxs-lookup"><span data-stu-id="2a3ee-109">PowerShell</span></span>

<span data-ttu-id="2a3ee-110">-Роль "org-Marketplace додатків"-GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="2a3ee-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="2a3ee-111">У результатах пошуку Get-Управліннярольова призначення, перегляньте записи в стовпці ефективні користувачі.</span><span class="sxs-lookup"><span data-stu-id="2a3ee-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="2a3ee-112">Докладні відомості про синтаксис і [параметр див.](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment)</span><span class="sxs-lookup"><span data-stu-id="2a3ee-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 