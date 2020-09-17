---
title: 932 оновлення AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806060"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="99b6a-102">Оновлення "Azure AD Connect"</span><span class="sxs-lookup"><span data-stu-id="99b6a-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="99b6a-103">За замовчуванням автоматичне оновлення ввімкнуто для Azure AD Connect, що допомагає забезпечити роботу найновішої версії.</span><span class="sxs-lookup"><span data-stu-id="99b6a-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="99b6a-104">Щоб перевірити параметри автоматичного оновлення, скористайтеся командлетом **Get-ADSyncAutoUpgrade** в ЛАЗУРКОМУ AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="99b6a-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="99b6a-105">Командлет поверне одне з наведених нижче значень.</span><span class="sxs-lookup"><span data-stu-id="99b6a-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="99b6a-106">**Увімкнуто**: функція автоматичного оновлення ввімкнена.</span><span class="sxs-lookup"><span data-stu-id="99b6a-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="99b6a-107">**Вимкнуто**: автоматичне оновлення вимкнуто.</span><span class="sxs-lookup"><span data-stu-id="99b6a-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="99b6a-108">**Призупинено**: система більше не має права на отримання автоматичних оновлень.</span><span class="sxs-lookup"><span data-stu-id="99b6a-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="99b6a-109">Не можна настроїти це значення; це встановлено системою.</span><span class="sxs-lookup"><span data-stu-id="99b6a-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="99b6a-110">Докладні відомості наведено в статті [Автоматичне оновлення](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="99b6a-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="99b6a-111">Щоб завантажити найновішу версію служби Azure AD Connect, перейдіть на сторінку [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .</span><span class="sxs-lookup"><span data-stu-id="99b6a-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
