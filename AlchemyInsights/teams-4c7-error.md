---
title: Команди 4C7 Error
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796456"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="7a75b-102">4C7 помилка в Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="7a75b-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="7a75b-103">Ця помилка виникає через те, що Microsoft teams потребує автентифікації форм.</span><span class="sxs-lookup"><span data-stu-id="7a75b-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="7a75b-104">Під час розгортання служби Active Directory об'єднання Services (AD FS), форми автентифікації не ввімкнуто для інтрамережі за промовчанням.</span><span class="sxs-lookup"><span data-stu-id="7a75b-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="7a75b-105">Якщо не вдається виконати інтегровану автентифікацію Windows, буде запропоновано ввійти за допомогою форм автентифікації.</span><span class="sxs-lookup"><span data-stu-id="7a75b-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="7a75b-106">Щоб вирішити цю проблему, увімкніть автентифікацію форм за допомогою оснащення AD FS консолі керування Microsoft (MMC) на комп'ютері, який має локальну копію служби Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7a75b-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="7a75b-107">Щоб зробити це, виконайте такі дії.</span><span class="sxs-lookup"><span data-stu-id="7a75b-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="7a75b-108">В області переходів перейдіть до **політики автентифікації**.</span><span class="sxs-lookup"><span data-stu-id="7a75b-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="7a75b-109">У розділі **дії** в області відомостей виберіть пункт **редагувати глобальний первинний автентифікації**.</span><span class="sxs-lookup"><span data-stu-id="7a75b-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="7a75b-110">На вкладці **інтрамережі** виберіть **автентифікацію форм**.</span><span class="sxs-lookup"><span data-stu-id="7a75b-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="7a75b-111">Виберіть **OK** (або **Застосувати**).</span><span class="sxs-lookup"><span data-stu-id="7a75b-111">Select **OK** (or **Apply**).</span></span>