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
ms.openlocfilehash: 8ffa8f64019077034bc4fad61d1d843849c42898
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/13/2019
ms.locfileid: "31858981"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="597a7-102">Оновлення блакитні оголошення підключення</span><span class="sxs-lookup"><span data-stu-id="597a7-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="597a7-103">За промовчанням автоматичні оновлення ввімкнуто для Azure оголошення підключитися, яка дозволяє переконатися, що ви використовуєте останню версію.</span><span class="sxs-lookup"><span data-stu-id="597a7-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="597a7-104">Перевірити параметри автоматичного оновлення, використовуйте командлет **Get-ADSyncAutoUpgrade** в Azure оголошення PowerShell.</span><span class="sxs-lookup"><span data-stu-id="597a7-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="597a7-105">На командлета буде повертати одне з таких значень:</span><span class="sxs-lookup"><span data-stu-id="597a7-105">The cmdlet will return one of following values:</span></span> 

- <span data-ttu-id="597a7-106">**Увімкнуто**: увімкнуто автоматичне оновлення.</span><span class="sxs-lookup"><span data-stu-id="597a7-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="597a7-107">**Вимкнуто**: автоматичне оновлення вимкнено.</span><span class="sxs-lookup"><span data-stu-id="597a7-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="597a7-108">**Перерване**: система вже не мають права на отримання автоматичних оновлень.</span><span class="sxs-lookup"><span data-stu-id="597a7-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="597a7-109">Неможливо настроїти це значення; встановлених у системі.</span><span class="sxs-lookup"><span data-stu-id="597a7-109">You can't configure this value; it's set by the system.</span></span> 

<span data-ttu-id="597a7-110">Докладніше перегляньте статтю [автоматичного оновлення](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="597a7-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="597a7-111">Щоб завантажити останню версію Azure оголошення підключення, перейдіть на [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="597a7-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
