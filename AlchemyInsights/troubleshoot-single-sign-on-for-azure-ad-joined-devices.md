---
title: Виправлення неполадок із одинарним входом для пристроїв, підключених до мережі Azure
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037337"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a><span data-ttu-id="c7a4f-102">Виправлення неполадок із одинарним входом для пристроїв, підключених до мережі Azure</span><span class="sxs-lookup"><span data-stu-id="c7a4f-102">Troubleshoot Single-sign on for Azure AD Joined Devices</span></span>

<span data-ttu-id="c7a4f-103">Якщо у вас є локальна Служба Active Directory (AD), і ви хочете приєднатися до свого домену, до якого приєдналися комп'ютери з лазуровим ОГОЛОШЕННЯМ, можна виконати цю роботу, виконавши гібридне об'єднання Лазур.</span><span class="sxs-lookup"><span data-stu-id="c7a4f-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="c7a4f-104">[Планування гібридного використання служби "Блакитний" для Active Directory –](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) надання вам відповідних заходів для реалізації гібридного об'єднання Azure в навколишньому середовищі.</span><span class="sxs-lookup"><span data-stu-id="c7a4f-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

<span data-ttu-id="c7a4f-105">Докладні відомості наведено в статті [Настроювання пристроїв AZURE AD для локального Single-Sign з використанням Windows Hello для бізнесу](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span><span class="sxs-lookup"><span data-stu-id="c7a4f-105">For more information, see [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="c7a4f-106">**Проблеми з основним маркером оновлення (PRT)**</span><span class="sxs-lookup"><span data-stu-id="c7a4f-106">**Primary Refresh Token (PRT) issues**</span></span>

<span data-ttu-id="c7a4f-107">Основний маркер оновлення (PRT) – ключовий артефакт автентифікації в Azure AD в ОС Windows 10, Windows Server 2016 і новіших версіях, iOS і Android.</span><span class="sxs-lookup"><span data-stu-id="c7a4f-107">A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="c7a4f-108">Це веб-маркер JSON (JWT), спеціально виданий для брокерів від корпорації Майкрософт першого учасника, щоб активувати єдиний вхід (SSO) через програми, які використовуються на цих пристроях.</span><span class="sxs-lookup"><span data-stu-id="c7a4f-108">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="c7a4f-109">Докладні відомості про те, як видається ГВП, використовується та захищена на пристроях з ОС Windows 10, Дізнайтеся, [що таке первинний маркер оновлення?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="c7a4f-109">For details on how a PRT is issued, used, and protected on Windows 10 devices, see [What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="c7a4f-110">**WamDefaultSet набору: так і AzureADPrt: так**</span><span class="sxs-lookup"><span data-stu-id="c7a4f-110">**WamDefaultSet: YES and AzureADPrt: YES**</span></span>

<span data-ttu-id="c7a4f-111">Ці поля вказують, чи користувач успішно автентифіковано для Azure AD під час входу на пристрій.</span><span class="sxs-lookup"><span data-stu-id="c7a4f-111">These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="c7a4f-112">Якщо значення **немає**, це може бути пов'язано з такими значеннями:</span><span class="sxs-lookup"><span data-stu-id="c7a4f-112">If the values are **NO**, it could be due to:</span></span>

- <span data-ttu-id="c7a4f-113">Хибний ключ сховища в модулі TPM, пов'язаний із пристроєм під час реєстрації (перевірка KeySignTest під час роботи з підвищеною)</span><span class="sxs-lookup"><span data-stu-id="c7a4f-113">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)</span></span>
- <span data-ttu-id="c7a4f-114">Альтернативний ІДЕНТИФІКАТОР входу</span><span class="sxs-lookup"><span data-stu-id="c7a4f-114">Alternate Login ID</span></span>
- <span data-ttu-id="c7a4f-115">Проксі-сервер HTTP не знайдено</span><span class="sxs-lookup"><span data-stu-id="c7a4f-115">HTTP Proxy not found</span></span>

<span data-ttu-id="c7a4f-116">Щоб виправити неполадки на пристроях за допомогою команди dsregcmd, ознайомтеся з пунктом " [стан єдиного входу](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)".</span><span class="sxs-lookup"><span data-stu-id="c7a4f-116">To troubleshoot devices using the dsregcmd command, see [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>
