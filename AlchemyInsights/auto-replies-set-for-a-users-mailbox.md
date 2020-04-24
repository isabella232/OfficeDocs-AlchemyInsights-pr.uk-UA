---
title: Налаштування автовідповідей для поштової скриньки
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 4ffe8d77dad7db5fd5806fe879cf4934e5ca7c4a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/23/2020
ms.locfileid: "43788903"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="05eb5-102">Налаштування автовідповідей для поштової скриньки користувача</span><span class="sxs-lookup"><span data-stu-id="05eb5-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="05eb5-103">**Спосіб 1**</span><span class="sxs-lookup"><span data-stu-id="05eb5-103">**Method 1**</span></span>

1. <span data-ttu-id="05eb5-104">Увійдіть на портал Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="05eb5-104">Sign in to the Microsoft 365 portal.</span></span>

2. <span data-ttu-id="05eb5-105">Виберіть **Користувачів > Активні користувачі** (або **Групи > Спільні поштові скриньки**, якщо цю функцію встановлено у спільній поштовій скриньці).</span><span class="sxs-lookup"><span data-stu-id="05eb5-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="05eb5-106">Виберіть користувача з поштовою скринькою Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="05eb5-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="05eb5-107">У спливаючому меню праворуч перейдіть до розділу **Параметри пошти > Автовідповіді** (якщо це спільна поштова скринька, відразу клацніть **Автовідповіді**).</span><span class="sxs-lookup"><span data-stu-id="05eb5-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="05eb5-108">**Спосіб 2**</span><span class="sxs-lookup"><span data-stu-id="05eb5-108">**Method 2**</span></span>

1. <span data-ttu-id="05eb5-109">Увійдіть на портал адміністрування Microsoft 365, використовуючи облікові дані адміністратора.</span><span class="sxs-lookup"><span data-stu-id="05eb5-109">Sign in to the Microsoft 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="05eb5-110">Розгорніть **Центри адміністрування** та клацніть **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="05eb5-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="05eb5-111">Клацніть зображення у верхньому правому куті, виберіть пункт**Інший користувач**, та виберіть поштову скриньку користувача, яку потрібно змінити.</span><span class="sxs-lookup"><span data-stu-id="05eb5-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="05eb5-112">У лівій частині виберіть **Параметри**, клацніть **Упорядкування електронної пошти**, а потім виберіть пункт **Автовідповіді.**</span><span class="sxs-lookup"><span data-stu-id="05eb5-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="05eb5-113">**Спосіб 3**</span><span class="sxs-lookup"><span data-stu-id="05eb5-113">**Method 3**</span></span>

<span data-ttu-id="05eb5-114">Запустіть наступний cmdlet у службі Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="05eb5-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="05eb5-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="05eb5-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="05eb5-116">Докладні відомості про cmdlet див. в [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="05eb5-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
