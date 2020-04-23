---
title: 932 оновлення AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766514"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="1dd24-102">Оновлення Azure AD-підключення</span><span class="sxs-lookup"><span data-stu-id="1dd24-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="1dd24-103">За промовчанням автоматичне оновлення увімкнуто для Azure AD-підключення, який допомагає переконатися, що ви використовуєте останню версію.</span><span class="sxs-lookup"><span data-stu-id="1dd24-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="1dd24-104">Щоб перевірити настройки автоматичного оновлення, використовуйте командлет **Get-Adsyncautокупності** в Azure AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="1dd24-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="1dd24-105">Командлет повертатиме одне з таких значень:</span><span class="sxs-lookup"><span data-stu-id="1dd24-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="1dd24-106">**Увімкнуто**: автоматичне оновлення увімкнуто.</span><span class="sxs-lookup"><span data-stu-id="1dd24-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="1dd24-107">**Вимкнуто**: автоматичне оновлення вимкнуто.</span><span class="sxs-lookup"><span data-stu-id="1dd24-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="1dd24-108">**Призупинено**: система більше не має права на отримання автоматичних оновлень.</span><span class="sxs-lookup"><span data-stu-id="1dd24-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="1dd24-109">Не можна настроїти це значення; вона встановлюється системою.</span><span class="sxs-lookup"><span data-stu-id="1dd24-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="1dd24-110">Докладніші відомості наведено в [режимі автоматичного оновлення](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="1dd24-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="1dd24-111">Щоб завантажити останню версію Azure AD-підключення, перейдіть до [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="1dd24-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
