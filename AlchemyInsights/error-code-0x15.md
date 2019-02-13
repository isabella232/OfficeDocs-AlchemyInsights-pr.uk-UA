---
title: Код помилки 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: У разі появи повідомлення про помилку під час активації Office 2013 віддалений робочий стіл служб (РДС) розгортання, розглянути питання про включення ADAL шляхом редагування реєстру.
ms.openlocfilehash: 6d4076ecb5c6ee3c3cf4c4610ad4aa29ab477d8a
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29929116"
---
<span data-ttu-id="a2739-103">У разі появи повідомлення про помилку під час активації Office 2013 віддалений робочий стіл служб (РДС) розгортання, розглянути питання про включення ADAL шляхом редагування реєстру.</span><span class="sxs-lookup"><span data-stu-id="a2739-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="a2739-104">**Ключ реєстру**</span><span class="sxs-lookup"><span data-stu-id="a2739-104">**Registry key**</span></span>|<span data-ttu-id="a2739-105">**Тип**</span><span class="sxs-lookup"><span data-stu-id="a2739-105">**Type**</span></span>|<span data-ttu-id="a2739-106">**Значення**</span><span class="sxs-lookup"><span data-stu-id="a2739-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="a2739-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="a2739-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="a2739-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="a2739-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="a2739-109">1</span><span class="sxs-lookup"><span data-stu-id="a2739-109">1</span></span>  <br/> |
   
<span data-ttu-id="a2739-110">Докладніше перегляньте [Увімкнути сучасних автентикації Office 2013 на пристроях Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="a2739-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="a2739-p101">АДАЛІЯ типово увімкнено у Office 365 ProPlus і Office 2016. > віддалений робочий стіл служб (РДС) була названа служб терміналів.</span><span class="sxs-lookup"><span data-stu-id="a2739-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

