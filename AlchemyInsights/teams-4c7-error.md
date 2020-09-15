---
title: Помилка 4C7 для команд
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
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700224"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="4a198-102">Помилка 4C7 в командах Microsoft</span><span class="sxs-lookup"><span data-stu-id="4a198-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="4a198-103">Ця помилка виникає через те, що команди Microsoft потребують автентифікації форм.</span><span class="sxs-lookup"><span data-stu-id="4a198-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="4a198-104">Якщо розгорнути служби Федерації Active Directory (AD FS), автентифікація форм не активовано для інтрамережі за замовчуванням.</span><span class="sxs-lookup"><span data-stu-id="4a198-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="4a198-105">Якщо Windows інтегровану автентифікацію не вдасться, з'явиться запит на вхід за допомогою автентифікації форм.</span><span class="sxs-lookup"><span data-stu-id="4a198-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="4a198-106">Щоб вирішити цю проблему, увімкніть автентифікацію форм за допомогою оснастки консолі керування РЕКЛАМНИМИ FS Microsoft (MMC) на комп'ютері, на якому використовується Локальна копія Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4a198-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="4a198-107">Щоб зробити це, виконайте такі дії.</span><span class="sxs-lookup"><span data-stu-id="4a198-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="4a198-108">В області переходів перейдіть до **політики автентифікації**.</span><span class="sxs-lookup"><span data-stu-id="4a198-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="4a198-109">У розділі **дії** в області відомостей виберіть пункт **редагування глобальної основної автентифікації**.</span><span class="sxs-lookup"><span data-stu-id="4a198-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="4a198-110">На вкладці **інтрамережа** натисніть кнопку **автентифікація форми**.</span><span class="sxs-lookup"><span data-stu-id="4a198-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="4a198-111">Натисніть **кнопку OK** (або **Додати**).</span><span class="sxs-lookup"><span data-stu-id="4a198-111">Select **OK** (or **Apply**).</span></span>