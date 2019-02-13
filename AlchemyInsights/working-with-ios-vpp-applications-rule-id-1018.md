---
title: Робота з iOS очок VPP додатків правило Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 65b9a727171a7551068717f6327f15e1aa8e6bed
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29917517"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="b13c8-102">Робота з iOS очок VPP додатків</span><span class="sxs-lookup"><span data-stu-id="b13c8-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="b13c8-103">Читав, [як керувати iOS застосунки, придбані через обсяг купівлі програми з Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) щоб дізнатися про особливості, обмеження та кроки, щоб зробити використання Apple обсяг купівлі програми та підтримку для його в Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="b13c8-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span> 
  
 <span data-ttu-id="b13c8-104">**Поширених проблем:** "Я призначено застосунок очок VPP iOS мої користувачі, але не установка".</span><span class="sxs-lookup"><span data-stu-id="b13c8-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span> 
  
- <span data-ttu-id="b13c8-p101">Це може статися, якщо використання єдиного очок VPP маркера через декілька провайдерів мобільного пристрою управління. ВПП токени від Apple можна використовувати лише з одного постачальника. Якщо ви використовували очок VPP маркер з кількох джерел, потрібно повторно завантажувати токен до Intune.</span><span class="sxs-lookup"><span data-stu-id="b13c8-p101">This can happen if a single VPP token is used across multiple mobile device management providers. VPP tokens from Apple may only be used with one provider. If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>
    
- <span data-ttu-id="b13c8-p102">Установка може також виникає, якщо загальна кількість установок перевищує кількість ліцензій. Щоб переглянути використання звіт для вашої ліцензії, перейдіть на **Intune мобільних додатків** \> **ліцензії застосунку** сторінки. Щоб відновити ліцензій на використання, розділ [цю статтю.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="b13c8-p102">The installation can also fail if the total number of installations exceed the number of licenses. To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page. To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
    

