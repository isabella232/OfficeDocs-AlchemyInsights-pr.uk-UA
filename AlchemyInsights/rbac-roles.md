---
title: 'Ролі RBAC '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583957"
---
# <a name="rbac-rules"></a><span data-ttu-id="38b04-102">Правила RBAC</span><span class="sxs-lookup"><span data-stu-id="38b04-102">RBAC rules</span></span>

<span data-ttu-id="38b04-103">Якщо з'являється повідомлення про помилку з дозволом:</span><span class="sxs-lookup"><span data-stu-id="38b04-103">If you get the permission error:</span></span> 

- <span data-ttu-id="38b04-104">**Клієнт із ідентифікатором об'єкта не має дозволу на виконання дій над областю (код: не вдалося знайти)**: під час спроби створити ресурс переконайтеся, що ви ввійшли в обліковий запис користувача, якому призначено роль, яка має право на записування до ресурсу в вибраній області.</span><span class="sxs-lookup"><span data-stu-id="38b04-104">**The client with object id does not have authorization to perform action over scope (code: AuthorizationFailed)**: when you try to create a resource, check that you are currently signed in with a user that is assigned a role that has write permission to the resource at the selected scope.</span></span> <span data-ttu-id="38b04-105">Наприклад, щоб керувати віртуальними машинами у групі ресурсів, необхідно мати роль [учасника віртуальної машини](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) в групі ресурсів (або батьківській області).</span><span class="sxs-lookup"><span data-stu-id="38b04-105">For example, to manage virtual machines in a resource group, you should have the [Virtual Machine Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) role on the resource group (or parent scope).</span></span> <span data-ttu-id="38b04-106">Список дозволів для кожної вбудованої ролі наведено [в статті вбудовані ролі для ресурсів Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="38b04-106">For a list of the permissions for each built-in role, see [Built-in roles for Azure resources](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="38b04-107">У **вас немає дозволу на створення запиту на підтримку**: під час спроби створити або оновити квиток служби підтримки переконайтеся, що ви зараз ввійшли в обліковий запис, який має роль Microsoft. підтримка/supportTickets/Write, як-от [вкладник "запит на підтримку](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)".</span><span class="sxs-lookup"><span data-stu-id="38b04-107">**You don't have permission to create a support request**: when you try to create or update a support ticket, check that you are currently signed in with a user that is assigned a role that has the Microsoft.Support/supportTickets/write permission, such as [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span></span>
- <span data-ttu-id="38b04-108">**Не можна створити більше призначень ролей (код: RoleAssignmentLimitExceeded)**: під час спроби призначити роль спробуйте зменшити кількість призначень ролей, призначаючи ролі до груп замість цього.</span><span class="sxs-lookup"><span data-stu-id="38b04-108">**No more role assignments can be created (code: RoleAssignmentLimitExceeded)**: when you try to assign a role, try to reduce the number of role assignments by assigning roles to groups instead.</span></span> <span data-ttu-id="38b04-109">Azure підтримує до завдань **2000** роль за передплатою.</span><span class="sxs-lookup"><span data-stu-id="38b04-109">Azure supports up to **2000** role assignments per subscription.</span></span>

<span data-ttu-id="38b04-110">Докладні відомості про ролі Блакитної RBAC наведено в статті [ролі БЛАКИТНОЇ RBAC](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="38b04-110">For more details on Azure RBAC roles, see [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
