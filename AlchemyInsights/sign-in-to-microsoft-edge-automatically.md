---
title: Автоматичне входу в Microsoft EDGE
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678820"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="52c13-102">Автоматичне входу в Microsoft EDGE</span><span class="sxs-lookup"><span data-stu-id="52c13-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="52c13-103">Microsoft EDGE використовує обліковий запис ОС за замовчуванням, щоб автоматично ввійти в користувача відповідно до способу настроювання пристрою користувача.</span><span class="sxs-lookup"><span data-stu-id="52c13-103">Microsoft Edge uses the OS's default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="52c13-104">Нижче описано сценарії кожного типу конфігурації пристрою та його залежного процесу для реєстрації користувачів:</span><span class="sxs-lookup"><span data-stu-id="52c13-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

1. <span data-ttu-id="52c13-105">**Пристрій Hybrid/AAD-J**: цей параметр доступний у Windows 10, на рівні вікна та відповідні версії сервера.</span><span class="sxs-lookup"><span data-stu-id="52c13-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="52c13-106">Користувачі автоматично мають доступ до своїх облікових записів "Azure Active Directory (AD)".</span><span class="sxs-lookup"><span data-stu-id="52c13-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
2. <span data-ttu-id="52c13-107">**Пристрій входить до складу домену**: цей параметр доступний у Windows 10, на рівні вікна, і відповідні версії сервера.</span><span class="sxs-lookup"><span data-stu-id="52c13-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="52c13-108">За замовчуванням користувачі з обліковими записами доменів не мають автоматичного входу; Щоб увімкнути функцію автоматичного входу, скористайтеся політикою **ConfigureOnPremisesAccountAutoSignIn** .</span><span class="sxs-lookup"><span data-stu-id="52c13-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="52c13-109">Щоб увімкнути автоматичний вхід для користувачів із обліковими записами Azure AD, спробуйте гібридне приєднання до своїх пристроїв.</span><span class="sxs-lookup"><span data-stu-id="52c13-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
3. <span data-ttu-id="52c13-110">Обліковий **запис за замовчуванням операційної системи – це обліковий запис Microsoft**: цей параметр доступний у Windows 10 RS3 (версія 1709, збірка 10.0.16299) і пізніші версії.</span><span class="sxs-lookup"><span data-stu-id="52c13-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="52c13-111">На корпоративних пристроях навряд чи виникне ситуація.</span><span class="sxs-lookup"><span data-stu-id="52c13-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="52c13-112">Однак, якщо обліковий запис за замовчуванням для ОС – це обліковий запис Microsoft, Microsoft EDGE автоматично ввійде в користувача за допомогою облікового запису Microsoft.</span><span class="sxs-lookup"><span data-stu-id="52c13-112">However, if the OS's default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
