---
title: Виправлення неполадок із гібридним приєднанням до Microsoft Azure AD
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401928"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a><span data-ttu-id="fa7c1-102">Виправлення неполадок із гібридним приєднанням до Microsoft Azure AD</span><span class="sxs-lookup"><span data-stu-id="fa7c1-102">Troubleshoot Hybrid Azure AD join</span></span>

<span data-ttu-id="fa7c1-103">Настійно рекомендується переконатися, що пристрій має доступ до кінцевих точок служби реєстрації пристроїв під системним обліковим записом, використовуючи [сценарій перевірки підключення до служби реєстрації пристроїв](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span><span class="sxs-lookup"><span data-stu-id="fa7c1-103">Highly Recommended Ensure that a device can access Device Registration endpoints under the system account by using the [Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span></span>

1. <span data-ttu-id="fa7c1-104">Якщо ви вперше налаштовуєте реєстрацію пристрою, ознайомтеся зі [Вступом до керування пристроями в Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/), щоб дізнатися, як установити контроль Microsoft Azure AD над пристроєм.</span><span class="sxs-lookup"><span data-stu-id="fa7c1-104">If you are setting up device registrations for the first time, be sure to review I[ntroduction to device management in Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) to learn how to get devices under the control of Azure AD.</span></span>
1. <span data-ttu-id="fa7c1-105">Якщо ви реєструєте пристрій безпосередньо в Microsoft Azure AD, а потім в Intune, спочатку [налаштуйте Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) і переконайтеся в наявності [ліцензій](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="fa7c1-105">If you are registering devices into Azure AD directly and enrolling them into Intune, be sure that you've [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
1. <span data-ttu-id="fa7c1-106">Переконайтеся, що ви маєте право на виконання операцій в Microsoft Azure AD та в локальній службі Active Directory.</span><span class="sxs-lookup"><span data-stu-id="fa7c1-106">Ensure that you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="fa7c1-107">Тільки глобальний адміністратор Microsoft Azure AD може керувати параметрами реєстрації пристроїв.</span><span class="sxs-lookup"><span data-stu-id="fa7c1-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="fa7c1-108">Крім того, щоб налаштувати автоматичну реєстрацію в локальній службі Active Directory, вам потрібно мати права адміністратора служби Active Directory та AD FS (якщо застосовується).</span><span class="sxs-lookup"><span data-stu-id="fa7c1-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="fa7c1-109">Додаткові відомості про усунення потенційних проблем із гібридним приєднанням див. в статті [Виправлення неполадок із гібридним приєднанням](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current). Щоб налаштувати гібридне приєднання до Microsoft Azure AD та керувати пристроями за допомогою порталу Microsoft Azure AD, див. статті [Налаштування пристроїв із гібридним приєднанням до Microsoft Azure AD (приєднаних до локального домену)](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) та [Керування пристроями за допомогою порталу Microsoft Azure](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="fa7c1-109">For more details on resolve potential issues with Hybrid join, see [Troubleshoot Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) for set up hybrid Azure AD joined and Manage Devices using Azure Ad portal, see [Set up hybrid Azure AD joined (on-premises domain-joined) devices](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) and [Manage devices using the Azure portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="fa7c1-110">Щоб усунути поширені проблеми з гібридним приєднанням до Microsoft Azure Active Directory (AD), див. статтю [Гібридне приєднання до Microsoft Azure AD: запитання й вiдповiдi](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span><span class="sxs-lookup"><span data-stu-id="fa7c1-110">To resolve common issues with Hybrid Azure Active Directory (AD) join, see [Hybrid Azure AD join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span></span>
