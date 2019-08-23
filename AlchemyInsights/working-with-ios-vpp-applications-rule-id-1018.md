---
title: Робота з iOS очок VPP додатків правило Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: a0bbc1f49f251ef4f16300c8cca98e219008d17e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36558026"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="b8d2a-102">Робота з iOS очок VPP додатків</span><span class="sxs-lookup"><span data-stu-id="b8d2a-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="b8d2a-103">Читав, [як керувати iOS застосунки, придбані через обсяг купівлі програми з Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) щоб дізнатися про особливості, обмеження та кроки, щоб зробити використання Apple обсяг купівлі програми та підтримку для його в Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="b8d2a-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="b8d2a-104">**Поширених проблем:** "Я призначено застосунок очок VPP iOS мої користувачі, але не установка".</span><span class="sxs-lookup"><span data-stu-id="b8d2a-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="b8d2a-105">Це може статися, якщо використання єдиного очок VPP маркера через декілька провайдерів мобільного пристрою управління.</span><span class="sxs-lookup"><span data-stu-id="b8d2a-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="b8d2a-106">ВПП токени від Apple можна використовувати лише з одного постачальника.</span><span class="sxs-lookup"><span data-stu-id="b8d2a-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="b8d2a-107">Якщо ви використовували очок VPP маркер з кількох джерел, потрібно повторно завантажувати токен до Intune.</span><span class="sxs-lookup"><span data-stu-id="b8d2a-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="b8d2a-108">Установка може також виникає, якщо загальна кількість установок перевищує кількість ліцензій.</span><span class="sxs-lookup"><span data-stu-id="b8d2a-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="b8d2a-109">Щоб переглянути використання звіт для вашої ліцензії, перейдіть на **Intune мобільних додатків** \> **ліцензії застосунку** сторінки.</span><span class="sxs-lookup"><span data-stu-id="b8d2a-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="b8d2a-110">Щоб відновити ліцензій на використання, розділ [цю статтю.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="b8d2a-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
