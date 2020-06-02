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
ms.openlocfilehash: 468d13e59602cf173ed2e17af44c66babfc28703
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506867"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="f3c04-103">Помилка під час активації Office 2013 на службах віддалених робочих столів</span><span class="sxs-lookup"><span data-stu-id="f3c04-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="f3c04-104">Якщо ви отримуєте повідомлення про помилку під час активації Office 2013 на розгортання служб віддалених робочих столів (RDS), спробуйте увімкнути ADAL, редагуючи реєстр.</span><span class="sxs-lookup"><span data-stu-id="f3c04-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="f3c04-105">**Реєстру**</span><span class="sxs-lookup"><span data-stu-id="f3c04-105">**Registry key**</span></span>|<span data-ttu-id="f3c04-106">**Тип**</span><span class="sxs-lookup"><span data-stu-id="f3c04-106">**Type**</span></span>|<span data-ttu-id="f3c04-107">**Значення**</span><span class="sxs-lookup"><span data-stu-id="f3c04-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f3c04-108">HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="f3c04-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="f3c04-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="f3c04-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="f3c04-110">1</span><span class="sxs-lookup"><span data-stu-id="f3c04-110">1</span></span>  <br/> |

<span data-ttu-id="f3c04-111">Щоб отримати додаткові відомості див. [Увімкнення сучасних автентифікації для Office 2013 на пристроях Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="f3c04-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="f3c04-112">ADAL увімкнуто за промовчанням у програмах Microsoft 365 для підприємств і Office 2016.</span><span class="sxs-lookup"><span data-stu-id="f3c04-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="f3c04-113">Служби віддалених робочих столів (RDS) раніше називали служби терміналів.</span><span class="sxs-lookup"><span data-stu-id="f3c04-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  