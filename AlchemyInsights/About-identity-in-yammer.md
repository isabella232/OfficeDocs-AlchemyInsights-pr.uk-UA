---
title: Відомості про ідентичність у Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664191"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="9ccd1-102">Відомості про ідентичність у Yammer</span><span class="sxs-lookup"><span data-stu-id="9ccd1-102">About identity in Yammer</span></span>

<span data-ttu-id="9ccd1-103">Рекомендується, щоб усі мережі могли уникнути проблем, пов'язаних із ідентифікацією в цій статті.</span><span class="sxs-lookup"><span data-stu-id="9ccd1-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="9ccd1-104">Забезпечення ідентифікації Office 365 після підготовки облікових записів Microsoft 365 для користувачів у Azure AD для того, щоб усі користувачі ввійшли за допомогою основного облікового запису Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9ccd1-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="9ccd1-105">Докладні відомості наведено в статті [застосування ідентифікації Office 365 для користувачів Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="9ccd1-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="9ccd1-106">Об'єднання кількох мереж Yammer.</span><span class="sxs-lookup"><span data-stu-id="9ccd1-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="9ccd1-107">Успадковане настроювання Yammer дозволяє декільком мережі Yammer підключатися до одного клієнта.</span><span class="sxs-lookup"><span data-stu-id="9ccd1-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="9ccd1-108">Докладні відомості наведено в статті [перенесення мережі – об'єднання кількох мереж Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="9ccd1-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="9ccd1-109">За потреби можна забезпечити ліцензування для Yammer, щоб заблокувати користувачів Yammer, якщо вони не мають ліцензії.</span><span class="sxs-lookup"><span data-stu-id="9ccd1-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="9ccd1-110">Докладні відомості наведено в статті [керування ліцензіями користувачів Yammer в Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="9ccd1-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="9ccd1-111">Нарешті, аудит списку користувачів для старих мереж Yammer та призупинення успадкованих користувачів.</span><span class="sxs-lookup"><span data-stu-id="9ccd1-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="9ccd1-112">Рекомендується призупиняти (деактивування) користувачів, а не видаляти їх, оскільки видалення незворотні.</span><span class="sxs-lookup"><span data-stu-id="9ccd1-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="9ccd1-113">Щоб отримати докладні відомості, ознайомтеся з [користувачами служби аудиту Yammer в мережах, підключених до Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) і [видаляти користувачів](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="9ccd1-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="9ccd1-114">Настроївши Yammer, виконавши наведені нижче дії, ви також зможете налаштувати мережу Yammer в рідному режимі для Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9ccd1-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="9ccd1-115">Докладні відомості наведено в статті [Настроювання мережі Yammer в рідному режимі для Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="9ccd1-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>