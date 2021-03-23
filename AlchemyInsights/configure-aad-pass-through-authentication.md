---
title: Настроювання автентифікації в надбудові "Azure Active Directory"
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6970"
- "9003915"
ms.openlocfilehash: be993b1f22d89a92afb099937dae815dc9c09e0e
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037535"
---
# <a name="configure-azure-active-directory-pass-through-authentication"></a><span data-ttu-id="14eed-102">Настроювання автентифікації в надбудові "Azure Active Directory"</span><span class="sxs-lookup"><span data-stu-id="14eed-102">Configure Azure Active Directory pass-through authentication</span></span>

<span data-ttu-id="14eed-103">Нижче наведено кілька посібників, які допоможуть настроїти автентифікацію через передавання.</span><span class="sxs-lookup"><span data-stu-id="14eed-103">Here are some guides to help you configure pass-through authentication:</span></span>

- <span data-ttu-id="14eed-104">**Щоб настроїти підключення Azure Active Directory**, виконайте такі дії: [синхронізація користувачів зі службою каталогів](https://admin.microsoft.com/AdminPortal/Home) дає змогу настроїти синхронізацію хеш-пароля або пройти автентифікацію.</span><span class="sxs-lookup"><span data-stu-id="14eed-104">**To set up Azure Active Directory Connect**: The [Sync users to your directory](https://admin.microsoft.com/AdminPortal/Home) guide helps you configure password hash synchronization or pass-through authentication.</span></span> <span data-ttu-id="14eed-105">Ця конфігурація дає змогу користувачам входити в електронну пошту та локальну службу Active Directory (контролер домену), використовуючи той самий пароль.</span><span class="sxs-lookup"><span data-stu-id="14eed-105">This configuration enables users to sign in to their email and to your on-premises Active Directory (domain controller) using the same password.</span></span>  <span data-ttu-id="14eed-106">У посібнику [користувача синхронізація](https://admin.microsoft.com/AdminPortal/Home) також описано вхід до системи за допомогою служб Федерації Active Directory (AD FS).</span><span class="sxs-lookup"><span data-stu-id="14eed-106">The [Sync users to your directory](https://admin.microsoft.com/AdminPortal/Home) guide also covers federation sign-in with Active Directory Federation Services (AD FS), too.</span></span>

- <span data-ttu-id="14eed-107">**Щоб настроїти функції Azure**: [посібник із настроювання лазурому](https://admin.microsoft.com/adminportal/home#/modernonboarding/azureadsetup) дає змогу настроїти функції в полі "простий", наприклад, "керування доступом на основі груп", "скидання пароля" для хмарних програм, а також проксі-сервер застосунку для публікування локальних веб-програм.</span><span class="sxs-lookup"><span data-stu-id="14eed-107">**To set up Azure features**: The [Azure AD setup guide](https://admin.microsoft.com/adminportal/home#/modernonboarding/azureadsetup) walks you through setting up the features in Azure Active Directory Basic, like group-based access management, self-service password reset for cloud apps, and Azure Active Directory Application Proxy for publishing on-premises web apps.</span></span>


