---
title: Код помилки 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: У разі появи повідомлення про помилку під час активації Office 2013 віддалений робочий стіл служб (РДС) розгортання, розглянути питання про включення ADAL шляхом редагування реєстру.
ms.openlocfilehash: 4ef2943e5a529368fa2c614e4431cf180924fbb8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527091"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="003ac-103">Помилка під час активації Office 2013 на служби віддалених робочих столів</span><span class="sxs-lookup"><span data-stu-id="003ac-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="003ac-104">У разі появи повідомлення про помилку під час активації Office 2013 віддалений робочий стіл служб (РДС) розгортання, розглянути питання про включення ADAL шляхом редагування реєстру.</span><span class="sxs-lookup"><span data-stu-id="003ac-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="003ac-105">**Ключ реєстру**</span><span class="sxs-lookup"><span data-stu-id="003ac-105">**Registry key**</span></span>|<span data-ttu-id="003ac-106">**Тип**</span><span class="sxs-lookup"><span data-stu-id="003ac-106">**Type**</span></span>|<span data-ttu-id="003ac-107">**Значення**</span><span class="sxs-lookup"><span data-stu-id="003ac-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="003ac-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="003ac-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="003ac-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="003ac-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="003ac-110">1</span><span class="sxs-lookup"><span data-stu-id="003ac-110">1</span></span>  <br/> |

<span data-ttu-id="003ac-111">Докладніше перегляньте [Увімкнути сучасних автентикації Office 2013 на пристроях Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="003ac-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="003ac-112">АДАЛІЯ типово увімкнено у Office 365 ProPlus і Office 2016.</span><span class="sxs-lookup"><span data-stu-id="003ac-112">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="003ac-113">Віддалений робочий стіл служб (РДС) була названа служб терміналів.</span><span class="sxs-lookup"><span data-stu-id="003ac-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  