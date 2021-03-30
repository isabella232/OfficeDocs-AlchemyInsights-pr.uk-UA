---
title: Single-Sign для пристроїв, підключених до Azure Active Directory
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405665"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a><span data-ttu-id="31982-102">Єдиний вхід для пристроїв, підключених до Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="31982-102">Single-sign on for Azure Active Directory Joined Devices</span></span>

<span data-ttu-id="31982-103">Якщо у вас є локальне середовище Active Directory (AD) і ви хочете приєднатися до комп'ютерів, приєднаних до домену, до Azure AD, це можна зробити, виконавши гібридне приєднання Azure AD.</span><span class="sxs-lookup"><span data-stu-id="31982-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="31982-104">[Інструкції.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) Сплануйте гібридне впровадження Azure Active Directory, виконавши відповідні кроки, щоб реалізувати гібридне об'єднання Azure AD у вашому середовищі.</span><span class="sxs-lookup"><span data-stu-id="31982-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

[<span data-ttu-id="31982-105">Налаштування приєднаних пристроїв до Azure AD для локальних Single-Sign за допомогою Windows Hello для бізнесу</span><span class="sxs-lookup"><span data-stu-id="31982-105">Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business</span></span>](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

<span data-ttu-id="31982-106">**Проблеми з основним маркером оновлення (PRT)** Основний маркер оновлення (PRT) – це основний артефакт автентифікації Azure AD у Windows 10, Windows Server 2016 і пізніших версій, iOS і Android.</span><span class="sxs-lookup"><span data-stu-id="31982-106">**Primary Refresh Token (PRT) issues** A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="31982-107">Це маркер JSON Web Token (JWT), який спеціально видано брошурам корпорації Майкрософт із маркерами першої сторони, щоб активувати єдиний вхід (SSO) для всіх програм, які використовуються на цих пристроях.</span><span class="sxs-lookup"><span data-stu-id="31982-107">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="31982-108">[У статті Що таке](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)основний маркер оновлення? ми надамо докладні відомості про те, як видано, використовується та захищається PRT на пристроях із Windows 10.</span><span class="sxs-lookup"><span data-stu-id="31982-108">[In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.</span></span>

<span data-ttu-id="31982-109">**WamDefaultSet: YES і AzureADPrt: YES** Ці поля вказують, чи користувач успішно автентифікувався в Azure AD під час входу на пристрій.</span><span class="sxs-lookup"><span data-stu-id="31982-109">**WamDefaultSet: YES and AzureADPrt: YES** These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="31982-110">Якщо значення мають значення **NO (НІ),** це може бути пов'язано з терміном виконання:</span><span class="sxs-lookup"><span data-stu-id="31982-110">If the values are **NO**, it could be due:</span></span>

- <span data-ttu-id="31982-111">Хибний ключ сховища в TPM, пов'язаному з пристроєм під час реєстрації (перевірте KeySignTest під час запуску влітку).</span><span class="sxs-lookup"><span data-stu-id="31982-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span></span>
- <span data-ttu-id="31982-112">Додатковий ідентифікатор входу</span><span class="sxs-lookup"><span data-stu-id="31982-112">Alternate Login ID</span></span>
- <span data-ttu-id="31982-113">Проксі-сервер HTTP не знайдено</span><span class="sxs-lookup"><span data-stu-id="31982-113">HTTP Proxy not found</span></span>

<span data-ttu-id="31982-114">Усунення несправностей пристроїв за допомогою команди dsregcmd – [стан єдиного входу](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="31982-114">Troubleshoot devices using the dsregcmd command - [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span></span>
