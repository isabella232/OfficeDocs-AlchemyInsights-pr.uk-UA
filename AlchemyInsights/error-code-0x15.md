---
title: Код помилки 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: У разі появи повідомлення про помилку під час активації Office 2013 віддалений робочий стіл служб (РДС) розгортання, розглянути питання про включення ADAL шляхом редагування реєстру.
ms.openlocfilehash: 89f9270169e13fd7706f7826c624ef8ae4d47b3f
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/15/2019
ms.locfileid: "28319298"
---
<span data-ttu-id="0d2b5-103">У разі появи повідомлення про помилку під час активації Office 2013 віддалений робочий стіл служб (РДС) розгортання, розглянути питання про включення ADAL шляхом редагування реєстру.</span><span class="sxs-lookup"><span data-stu-id="0d2b5-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="0d2b5-104">**Ключ реєстру**</span><span class="sxs-lookup"><span data-stu-id="0d2b5-104">**Registry key**</span></span>|<span data-ttu-id="0d2b5-105">**Тип**</span><span class="sxs-lookup"><span data-stu-id="0d2b5-105">**Type**</span></span>|<span data-ttu-id="0d2b5-106">**Значення**</span><span class="sxs-lookup"><span data-stu-id="0d2b5-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="0d2b5-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="0d2b5-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="0d2b5-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="0d2b5-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="0d2b5-109">1</span><span class="sxs-lookup"><span data-stu-id="0d2b5-109">1</span></span>  <br/> |
   
<span data-ttu-id="0d2b5-110">Докладніше перегляньте [Увімкнути сучасних автентикації Office 2013 на пристроях Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="0d2b5-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="0d2b5-p101">АДАЛІЯ типово увімкнено у Office 365 ProPlus і Office 2016. > Послуги віддаленого робочого столу (RDS) була названа служб терміналів.</span><span class="sxs-lookup"><span data-stu-id="0d2b5-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

