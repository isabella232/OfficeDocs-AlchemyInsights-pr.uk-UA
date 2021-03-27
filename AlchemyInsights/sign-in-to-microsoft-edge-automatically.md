---
title: Автоматичний вхід у Microsoft Edge
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
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398750"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="62333-102">Автоматичний вхід у Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="62333-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="62333-103">Microsoft Edge використовує стандартний обліковий запис ОС, щоб автоматично входити в обліковий запис відповідно до настройок пристрою користувача.</span><span class="sxs-lookup"><span data-stu-id="62333-103">Microsoft Edge uses the OS default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="62333-104">Нижче описано сценарії конфігурації кожного типу пристрою та залежні від користувача процедури входу.</span><span class="sxs-lookup"><span data-stu-id="62333-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

- <span data-ttu-id="62333-105">**Пристрій гібридний/AAD-J:** цей параметр доступний у Windows 10, нижче рівня Windows і у відповідних версіях сервера.</span><span class="sxs-lookup"><span data-stu-id="62333-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="62333-106">Користувачі автоматично ввійшли за допомогою облікових записів Azure Active Directory (AD).</span><span class="sxs-lookup"><span data-stu-id="62333-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
- <span data-ttu-id="62333-107">**Пристрій приєднано до** домену: цей параметр доступний у Windows 10, на рівні нижче Windows і у відповідних версіях сервера.</span><span class="sxs-lookup"><span data-stu-id="62333-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="62333-108">За замовчуванням користувачі з обліковими записами домену не ввійшли автоматично. щоб увімкнути автоматичний вхід до них, скористайтеся політикою **ConfigureOnPremisesAccountAutoSignIn.**</span><span class="sxs-lookup"><span data-stu-id="62333-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="62333-109">Щоб активувати автоматичний вхід для користувачів з обліковими записами Azure AD, реоюендуйте гібридне приєднання до своїх пристроїв.</span><span class="sxs-lookup"><span data-stu-id="62333-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
- <span data-ttu-id="62333-110">Обліковий запис Microsoft за замовчуванням використовується в ОС **Windows** 10 RS3 (версія 1709, збірка 10.0.16299) і новіших версіях.</span><span class="sxs-lookup"><span data-stu-id="62333-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="62333-111">Навпаки, цей сценарій має трапитися на корпоративних пристроях.</span><span class="sxs-lookup"><span data-stu-id="62333-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="62333-112">Однак, якщо за замовчуванням використовується обліковий запис Microsoft для ОС, Microsoft Edge автоматично ввійме в обліковий запис Microsoft.</span><span class="sxs-lookup"><span data-stu-id="62333-112">However, if the OS default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
