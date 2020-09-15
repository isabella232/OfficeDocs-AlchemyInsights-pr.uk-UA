---
title: Робота з програмами з iOS VPP для правил 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688967"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="037bb-102">Робота з застосунками iOS VPP</span><span class="sxs-lookup"><span data-stu-id="037bb-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="037bb-103">Дізнайтеся, [як керувати програмами з iOS, придбаними за допомогою програми для придбання, за допомогою Microsoft Inteune](https://docs.microsoft.com/intune/vpp-apps-ios) , щоб дізнатися про функції, обмеження та кроки, щоб використовувати програму придбання Apple, а також підтримку для неї в Microsoft InTune.</span><span class="sxs-lookup"><span data-stu-id="037bb-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="037bb-104">**Поширені проблеми:** "Я призначив програму iOS VPP для моїх користувачів, але Помилка інсталяції".</span><span class="sxs-lookup"><span data-stu-id="037bb-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="037bb-105">Це може статися, якщо один маркер VPP використовується в різних провайдерів керування мобільними пристроями.</span><span class="sxs-lookup"><span data-stu-id="037bb-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="037bb-106">Маркери VPP від Apple можна використовувати лише з одним постачальником.</span><span class="sxs-lookup"><span data-stu-id="037bb-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="037bb-107">Якщо ви використовували маркер VPP із кількома постачальниками, потрібно повторно передати маркер на веб-програму Inune.</span><span class="sxs-lookup"><span data-stu-id="037bb-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="037bb-108">Процес інсталяції також може не відповідувати, якщо загальна кількість інсталяцій перевищує кількість ліцензій.</span><span class="sxs-lookup"><span data-stu-id="037bb-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="037bb-109">Щоб переглянути звіт про використання ліцензій, перейдіть на сторінку ліцензії програми для **мобільних пристроїв програми inune** \> **App licenses** .</span><span class="sxs-lookup"><span data-stu-id="037bb-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="037bb-110">Щоб дізнатися, як відновити ліцензії у використанні, ознайомтеся з [цією статтею.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="037bb-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
