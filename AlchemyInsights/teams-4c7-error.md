---
title: Помилка Teams 4c7
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786690"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="ebc21-102">Помилка 4c7 у Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="ebc21-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="ebc21-103">Ця помилка виникає, тому що Microsoft Teams потребує автентифікації форм.</span><span class="sxs-lookup"><span data-stu-id="ebc21-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="ebc21-104">Під час розгортання служб об'єднання Active Directory (AD FS) для інтрамережі автентифікацію форм не активовано.</span><span class="sxs-lookup"><span data-stu-id="ebc21-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="ebc21-105">Якщо не вдається інтегрована автентифікація Windows, буде запропоновано ввійти за допомогою автентифікації форм.</span><span class="sxs-lookup"><span data-stu-id="ebc21-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="ebc21-106">Щоб вирішити цю проблему, увімкніть автентифікацію форм за допомогою консолі керування AD FS (MMC) на комп'ютері, де є локальна копія Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ebc21-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="ebc21-107">Щоб зробити це, виконайте такі дії.</span><span class="sxs-lookup"><span data-stu-id="ebc21-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="ebc21-108">В області переходів перейдіть до пункту Політики **автентифікації.**</span><span class="sxs-lookup"><span data-stu-id="ebc21-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="ebc21-109">У розділі **Дії** в області відомостей виберіть Редагувати глобальну **основну автентифікацію.**</span><span class="sxs-lookup"><span data-stu-id="ebc21-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="ebc21-110">На вкладці **Інтрамережа** виберіть Автентифікація **форм**.</span><span class="sxs-lookup"><span data-stu-id="ebc21-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="ebc21-111">Натисніть **кнопку OK** (або **Застосувати).**</span><span class="sxs-lookup"><span data-stu-id="ebc21-111">Select **OK** (or **Apply**).</span></span>