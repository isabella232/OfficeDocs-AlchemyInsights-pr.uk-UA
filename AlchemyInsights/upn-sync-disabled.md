---
title: UPN синхронізація вимкнуто
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 33bc7e30d41ff70e2ce55d946202acf45dbcb0f2
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726125"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="9d1ef-102">UPN синхронізація вимкнуто</span><span class="sxs-lookup"><span data-stu-id="9d1ef-102">UPN sync disabled</span></span>

<span data-ttu-id="9d1ef-103">Якщо ви почали синхронізацію з Azure AD до 30 березня, 2016, виконайте такі команди Azure AD PowerShell, щоб увімкнути UPN, м'який збіг лише для вашої організації:</span><span class="sxs-lookup"><span data-stu-id="9d1ef-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="9d1ef-104">**Набір-Mвійськовій функції-функція Вклюєтьеoftenonupn-увімкнути $True**</span><span class="sxs-lookup"><span data-stu-id="9d1ef-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="9d1ef-105">UPN Soft Match автоматично вмикається для організацій, які почали синхронізацію з Azure AD або після 30 березня 2016.</span><span class="sxs-lookup"><span data-stu-id="9d1ef-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="9d1ef-106">Щоб дізнатися більше про ввімкнення плавного зіставлення UPN та інших функцій для синхронізації, перегляньте [функції служби AZURE AD-підключення синхронізації](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="9d1ef-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

