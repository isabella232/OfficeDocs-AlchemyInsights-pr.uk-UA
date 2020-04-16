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
ms.openlocfilehash: aeeb2e1e76fe602d2767b422797452fd1155fdd5
ms.sourcegitcommit: fdfd41c2bfb2d45003b3906e6469377384a91cb5
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2020
ms.locfileid: "43509538"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="c836f-102">Налаштування автовідповідей для поштової скриньки користувача</span><span class="sxs-lookup"><span data-stu-id="c836f-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="c836f-103">**Спосіб 1**</span><span class="sxs-lookup"><span data-stu-id="c836f-103">**Method 1**</span></span>

1. <span data-ttu-id="c836f-104">Увійдіть на портал Office 365.</span><span class="sxs-lookup"><span data-stu-id="c836f-104">Sign in to the Office 365 portal.</span></span>

2. <span data-ttu-id="c836f-105">Виберіть **Користувачів > Активні користувачі** (або **Групи > Спільні поштові скриньки**, якщо цю функцію встановлено у спільній поштовій скриньці).</span><span class="sxs-lookup"><span data-stu-id="c836f-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="c836f-106">Виберіть користувача з поштовою скринькою Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="c836f-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="c836f-107">У спливаючому меню праворуч перейдіть до розділу **Параметри пошти > Автовідповіді** (якщо це спільна поштова скринька, відразу клацніть **Автовідповіді**).</span><span class="sxs-lookup"><span data-stu-id="c836f-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="c836f-108">**Спосіб 2**</span><span class="sxs-lookup"><span data-stu-id="c836f-108">**Method 2**</span></span>

1. <span data-ttu-id="c836f-109">Увійдіть на портал адміністрування Office 365, використовуючи облікові дані адміністратора.</span><span class="sxs-lookup"><span data-stu-id="c836f-109">Sign in to the Office 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="c836f-110">Розгорніть **Центри адміністрування** та клацніть **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="c836f-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="c836f-111">Клацніть зображення у верхньому правому куті, виберіть пункт**Інший користувач**, та виберіть поштову скриньку користувача, яку потрібно змінити.</span><span class="sxs-lookup"><span data-stu-id="c836f-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="c836f-112">У лівій частині виберіть **Параметри**, клацніть **Упорядкування електронної пошти**, а потім виберіть пункт **Автовідповіді.**</span><span class="sxs-lookup"><span data-stu-id="c836f-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="c836f-113">**Спосіб 3**</span><span class="sxs-lookup"><span data-stu-id="c836f-113">**Method 3**</span></span>

<span data-ttu-id="c836f-114">Запустіть наступний cmdlet у службі Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="c836f-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="c836f-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="c836f-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="c836f-116">Докладні відомості про cmdlet див. в [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="c836f-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
