---
title: 932 оновлення AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 0bbb847bb1381330065ebba6e109795908b06490
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/22/2019
ms.locfileid: "30778762"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="90d5f-102">Оновлення блакитні оголошення підключення</span><span class="sxs-lookup"><span data-stu-id="90d5f-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="90d5f-103">За промовчанням автоматичні оновлення ввімкнуто для Azure оголошення підключитися, яка дозволяє переконатися, що ви використовуєте останню версію.</span><span class="sxs-lookup"><span data-stu-id="90d5f-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="90d5f-104">Перевірити параметри автоматичного оновлення, використовуйте командлет **Get-ADSyncAutoUpgrade** в Azure оголошення PowerShell.</span><span class="sxs-lookup"><span data-stu-id="90d5f-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="90d5f-105">На командлета буде повертати одне з таких значень:</span><span class="sxs-lookup"><span data-stu-id="90d5f-105">The cmdlet will return one of following values:</span></span> 
  
- <span data-ttu-id="90d5f-106">**Увімкнуто**: увімкнуто автоматичне оновлення.</span><span class="sxs-lookup"><span data-stu-id="90d5f-106">**Enabled**: Automatic upgrade is enabled.</span></span> 
    
- <span data-ttu-id="90d5f-107">**Вимкнуто**: автоматичне оновлення вимкнено.</span><span class="sxs-lookup"><span data-stu-id="90d5f-107">**Disabled**: Automatic upgrade is disabled.</span></span> 
    
- <span data-ttu-id="90d5f-108">**Перерване**: система вже не мають права на отримання автоматичних оновлень.</span><span class="sxs-lookup"><span data-stu-id="90d5f-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="90d5f-109">Неможливо настроїти це значення; встановлених у системі.</span><span class="sxs-lookup"><span data-stu-id="90d5f-109">You can't configure this value; it's set by the system.</span></span> 
    
<span data-ttu-id="90d5f-110">Докладніше перегляньте статтю [автоматичного оновлення](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="90d5f-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>
  
<span data-ttu-id="90d5f-111">Щоб завантажити останню версію Azure оголошення підключення, перейдіть на [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="90d5f-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
  

