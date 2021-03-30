---
title: Усунення несправностей, пов'язаних із приєднанням до Azure
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
- "9003246"
- "6157"
ms.openlocfilehash: 0e9f7c95cf522340e9976f668c1d1a9eaff71910
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405765"
---
# <a name="troubleshoot-azure-ad-join-issues"></a><span data-ttu-id="f0eaf-102">Усунення несправностей, пов'язаних із приєднанням до Azure</span><span class="sxs-lookup"><span data-stu-id="f0eaf-102">Troubleshoot Azure AD join issues</span></span>

1. <span data-ttu-id="f0eaf-103">Якщо ви вперше настроєте реєстрацію пристроїв, перевірте загальні відомості про керування пристроями в [Azure Active Directory,](https://docs.microsoft.com/azure/active-directory/devices/overview) що допоможе вам отримати пристрої під контролем в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f0eaf-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="f0eaf-104">Якщо ви реєструєте пристрої безпосередньо в Azure AD та зареєстрували їх в Intune, переконайтеся, [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) що ви налаштували [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) і ліцензування настроїли спочатку.</span><span class="sxs-lookup"><span data-stu-id="f0eaf-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="f0eaf-105">Переконайтеся, що ви маєте право виконувати операції в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f0eaf-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="f0eaf-106">Лише глобальний адміністратор в Azure AD може керувати параметрами реєстрації пристроїв.</span><span class="sxs-lookup"><span data-stu-id="f0eaf-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="f0eaf-107">Відомості про те, як виконати приєднання до Azure AD, див. в [статтях Планування Azure AD Join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).</span><span class="sxs-lookup"><span data-stu-id="f0eaf-107">To do Azure AD join implementation, see [Plan Azure AD Join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="f0eaf-108">Докладні відомості про вирішення поширених проблем із приєднанням до Azure AD див. в статтях [Azure Ad Join:](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) запитання й відповіді та пристрій для Windows 10 pro див. в статті Не вдається приєднатися до комп'ютера з [Windows 10 Pro](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900) до Azure AD – Потрібно оновити до – Спільнота Microsoft</span><span class="sxs-lookup"><span data-stu-id="f0eaf-108">For more details on resolving  common issues with Azure AD join see [Azure Ad Join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)</span></span>
