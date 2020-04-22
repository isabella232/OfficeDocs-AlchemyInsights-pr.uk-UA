---
title: Код помилки 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Якщо ви отримуєте повідомлення про помилку під час активації Office 2013 на розгортання служб віддалених робочих столів (RDS), спробуйте увімкнути ADAL, редагуючи реєстр.
ms.openlocfilehash: 566d63cbe37d295b3546b9d7d5b14dfc8e8fe0ec
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703159"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="e37a1-103">Помилка під час активації Office 2013 на службах віддалених робочих столів</span><span class="sxs-lookup"><span data-stu-id="e37a1-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="e37a1-104">Якщо ви отримуєте повідомлення про помилку під час активації Office 2013 на розгортання служб віддалених робочих столів (RDS), спробуйте увімкнути ADAL, редагуючи реєстр.</span><span class="sxs-lookup"><span data-stu-id="e37a1-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="e37a1-105">**Реєстру**</span><span class="sxs-lookup"><span data-stu-id="e37a1-105">**Registry key**</span></span>|<span data-ttu-id="e37a1-106">**Тип**</span><span class="sxs-lookup"><span data-stu-id="e37a1-106">**Type**</span></span>|<span data-ttu-id="e37a1-107">**Значення**</span><span class="sxs-lookup"><span data-stu-id="e37a1-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="e37a1-108">HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="e37a1-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="e37a1-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="e37a1-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="e37a1-110">1</span><span class="sxs-lookup"><span data-stu-id="e37a1-110">1</span></span>  <br/> |

<span data-ttu-id="e37a1-111">Щоб отримати додаткові відомості див. [Увімкнення сучасних автентифікації для Office 2013 на пристроях Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="e37a1-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="e37a1-112">ADAL увімкнуто за промовчанням у програмах Microsoft 365 для підприємств і Office 2016.</span><span class="sxs-lookup"><span data-stu-id="e37a1-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="e37a1-113">Служби віддалених робочих столів (RDS) раніше називали служби терміналів.</span><span class="sxs-lookup"><span data-stu-id="e37a1-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  