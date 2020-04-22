---
title: Робота з iOS VPP додатків код правила 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719978"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="b7ff1-102">Робота з додатками iOS VPP</span><span class="sxs-lookup"><span data-stu-id="b7ff1-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="b7ff1-103">Прочитайте, [як керувати додатками iOS, придбаними через програму купівлі-продажу з Microsoft InTune](https://docs.microsoft.com/intune/vpp-apps-ios) , щоб дізнатися про функції, обмеження та кроки, щоб використовувати програму купівлі-продажу Apple і підтримку його в Microsoft InTune.</span><span class="sxs-lookup"><span data-stu-id="b7ff1-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="b7ff1-104">**Поширені проблеми:** "Я призначив додаток iOS VPP для моїх користувачів, але установка не вдалося."</span><span class="sxs-lookup"><span data-stu-id="b7ff1-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="b7ff1-105">Це може статися, якщо один маркер VPP використовується в кількох мобільних постачальників пристроїв керування.</span><span class="sxs-lookup"><span data-stu-id="b7ff1-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="b7ff1-106">Маркери VPP від Apple можуть використовуватися лише з одним постачальником.</span><span class="sxs-lookup"><span data-stu-id="b7ff1-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="b7ff1-107">Якщо ви використовували маркер VPP з кількома постачальниками, потрібно повторно завантажити маркер у InTune.</span><span class="sxs-lookup"><span data-stu-id="b7ff1-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="b7ff1-108">Інсталяція також може не вдатися, якщо загальна кількість встановлень перевищує кількість ліцензій.</span><span class="sxs-lookup"><span data-stu-id="b7ff1-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="b7ff1-109">Щоб переглянути звіт про використання для ліцензій, перейдіть на сторінку \> **ліцензії застосунку** для **мобільних додатків InTune** .</span><span class="sxs-lookup"><span data-stu-id="b7ff1-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="b7ff1-110">Щоб дізнатися, як відновити використання ліцензій, див [у цій статті.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="b7ff1-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
