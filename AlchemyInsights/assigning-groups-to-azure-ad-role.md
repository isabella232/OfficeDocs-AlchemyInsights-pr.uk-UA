---
title: Призначення груп для ролі Azure AD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885402"
---
# <a name="assigning-groups-to-azure-ad-role"></a><span data-ttu-id="243e2-102">Призначення груп для ролі Azure AD</span><span class="sxs-lookup"><span data-stu-id="243e2-102">Assigning groups to Azure AD role</span></span>

<span data-ttu-id="243e2-103">Щоб призначити групу Azure AD з джерелом повноважень у Лазурому, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="243e2-103">To assign an Azure AD group with source of authority in Azure AD to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="243e2-104">Створіть нову групу, щоб створити нову групу.</span><span class="sxs-lookup"><span data-stu-id="243e2-104">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="243e2-105">муніципалітет.</span><span class="sxs-lookup"><span data-stu-id="243e2-105">a.</span></span> <span data-ttu-id="243e2-106">Увійдіть у центр адміністрування Azure AD, щоб отримати **Привілейований адміністратор ролей** або **глобальні дозволи адміністратора** .</span><span class="sxs-lookup"><span data-stu-id="243e2-106">Sign in to the Azure AD admin center with **privileged role administrator** or **global administrator** permissions.</span></span>
    <span data-ttu-id="243e2-107">b.</span><span class="sxs-lookup"><span data-stu-id="243e2-107">b.</span></span> <span data-ttu-id="243e2-108">Виберіть **> групи Azure Active Directory > усі групи > нової групи**.</span><span class="sxs-lookup"><span data-stu-id="243e2-108">Select **Azure Active Directory > Groups > All groups > New group**.</span></span>
    <span data-ttu-id="243e2-109">c.</span><span class="sxs-lookup"><span data-stu-id="243e2-109">c.</span></span> <span data-ttu-id="243e2-110">Створіть групу.</span><span class="sxs-lookup"><span data-stu-id="243e2-110">Create the group.</span></span>

2. <span data-ttu-id="243e2-111">Призначте роль групі під час створення групи або після створення групи.</span><span class="sxs-lookup"><span data-stu-id="243e2-111">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="243e2-112">муніципалітет.</span><span class="sxs-lookup"><span data-stu-id="243e2-112">a.</span></span> <span data-ttu-id="243e2-113">Щоб призначити роль групі під час створення групи, перейдіть **до групи, щоб** перейти до неї, і створіть групу.</span><span class="sxs-lookup"><span data-stu-id="243e2-113">To assign a role to the group at the time of group creation, switch on the toggle **Azure AD roles can be assigned to the group** and create the group.</span></span>
    <span data-ttu-id="243e2-114">b.</span><span class="sxs-lookup"><span data-stu-id="243e2-114">b.</span></span> <span data-ttu-id="243e2-115">Щоб призначити роль групі після її створення, перейдіть до вкладки **призначені ролі** для новоствореної групи та призначте їй роль для групи.</span><span class="sxs-lookup"><span data-stu-id="243e2-115">To assign a role to the group after it has been created, navigate to the **Assigned roles** tab for the newly created group, and assign the role to the group.</span></span>  

<span data-ttu-id="243e2-116">**Керування членством групи, призначеної для ролі Azure AD**</span><span class="sxs-lookup"><span data-stu-id="243e2-116">**Manage membership of a group that is assigned to Azure AD role**</span></span>

<span data-ttu-id="243e2-117">Щоб уникнути підвищення привілеїв, за замовчуванням лише привілейовані адміністратори ролей і глобальні адміністратори можуть змінювати членство групи, призначеної для ролі.</span><span class="sxs-lookup"><span data-stu-id="243e2-117">To prevent elevation of privileges, by default, only privileged role administrators and global administrators can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="243e2-118">Однак вони можуть призначити власника для такої групи та делегувати це завдання.</span><span class="sxs-lookup"><span data-stu-id="243e2-118">They can, however, choose to assign an owner for such a group and delegate this task.</span></span>

<span data-ttu-id="243e2-119">Щоб отримати докладні відомості про призначення хмарних груп до ролей Azure AD, див. [призначення РОЛІ реклами до групи Cloud](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span><span class="sxs-lookup"><span data-stu-id="243e2-119">For more details on assigning cloud groups to Azure AD roles, see [Assign a AD roles to Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span> <span data-ttu-id="243e2-120">Докладні відомості про функції виправлення неполадок, призначені для хмарних груп, наведено в статті [усунення несправностей ролей, призначених для хмарних груп](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span><span class="sxs-lookup"><span data-stu-id="243e2-120">For more details on troubleshooting roles assigned to cloud groups, see [Troubleshoot roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>





