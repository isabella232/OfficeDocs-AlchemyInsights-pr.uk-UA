---
title: Розгортання групової політики
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/03/2021
ms.locfileid: "50428048"
---
# <a name="gpo-deployment"></a><span data-ttu-id="62e26-102">Розгортання групової політики</span><span class="sxs-lookup"><span data-stu-id="62e26-102">GPO Deployment</span></span>

<span data-ttu-id="62e26-103">Настройки для об'єктів користувача та комп'ютера в службах доменів "Лазурний" (Sure AD DS) часто керуються за допомогою об'єктів групової політики (GPS).</span><span class="sxs-lookup"><span data-stu-id="62e26-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="62e26-104">У Azure AD DS містяться вбудовані контейнери для користувачів AADDC і контейнерів для комп'ютерів AADDC.</span><span class="sxs-lookup"><span data-stu-id="62e26-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="62e26-105">Ви можете налаштувати ці вбудовані GPOs, щоб налаштувати групову політику, як потрібно для вашого середовища.</span><span class="sxs-lookup"><span data-stu-id="62e26-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="62e26-106">Користувачі групи «Адміністратори DC» мають права адміністрування групової політики в домені Azure AD DS, а також можуть створювати користувацькі та організаційні одиниці (OUs).</span><span class="sxs-lookup"><span data-stu-id="62e26-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="62e26-107">Докладні відомості про групову політику та її роботу наведено в статті [Огляд групової політики](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span><span class="sxs-lookup"><span data-stu-id="62e26-107">For more information on what group policy is and how it works, see [Group Policy Overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="62e26-108">У гібридному середовищі групові політики, настроєні в локальній середовищі AD DS, не синхронізуються з Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="62e26-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="62e26-109">Щоб визначити параметри конфігурації для користувачів або комп'ютерів у Azure AD DS, відредагуйте один із стандартних служб GPOs або створіть Настроюваний об'єкт групової політики.</span><span class="sxs-lookup"><span data-stu-id="62e26-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="62e26-110">У цій статті [керування груповою політикою](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) показано, як інсталювати засоби керування груповою політикою, як тон відредагувати вбудовану програму GTS, а також як створювати користувацькі служби gppos.</span><span class="sxs-lookup"><span data-stu-id="62e26-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>
