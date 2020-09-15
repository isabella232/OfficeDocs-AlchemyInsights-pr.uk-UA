---
title: Код помилки 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Якщо ви отримуєте повідомлення про помилку під час активації Office 2013 у розгортаннях служб віддалених робочих столів (RDS), радимо ввімкнути параметр ADAL, змінивши реєстр.
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709208"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="807c1-103">Помилка під час активації Office 2013 на віддалених настільних службах</span><span class="sxs-lookup"><span data-stu-id="807c1-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="807c1-104">Якщо ви отримуєте повідомлення про помилку під час активації Office 2013 у розгортаннях служб віддалених робочих столів (RDS), радимо ввімкнути параметр ADAL, змінивши реєстр.</span><span class="sxs-lookup"><span data-stu-id="807c1-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="807c1-105">**Розділ реєстру**</span><span class="sxs-lookup"><span data-stu-id="807c1-105">**Registry key**</span></span>|<span data-ttu-id="807c1-106">**Введіть**</span><span class="sxs-lookup"><span data-stu-id="807c1-106">**Type**</span></span>|<span data-ttu-id="807c1-107">**Значення**</span><span class="sxs-lookup"><span data-stu-id="807c1-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="807c1-108">HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="807c1-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="807c1-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="807c1-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="807c1-110">1</span><span class="sxs-lookup"><span data-stu-id="807c1-110">1</span></span>  <br/> |

<span data-ttu-id="807c1-111">Докладні відомості наведено в статті [Увімкнення сучасної автентифікації для Office 2013 на пристроях з ОС Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="807c1-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="807c1-112">Служба ADAL ввімкнена за замовчуванням у програмах Microsoft 365 для підприємств і Office 2016.</span><span class="sxs-lookup"><span data-stu-id="807c1-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="807c1-113">Служби віддалених настільних комп'ютерів (RDS) раніше були іменованими службами терміналів.</span><span class="sxs-lookup"><span data-stu-id="807c1-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  