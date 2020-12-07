---
title: Що робити, якщо функції Azure не працюють належним чином у Microsoft EDGE
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583778"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a><span data-ttu-id="25afd-102">Що робити, якщо функції Azure не працюють належним чином у Microsoft EDGE</span><span class="sxs-lookup"><span data-stu-id="25afd-102">What to do if Azure features don't work properly in Microsoft Edge</span></span>

<span data-ttu-id="25afd-103">Microsoft EDGE має [відомі проблеми](https://go.microsoft.com/fwlink/?linkid=2140608) , пов'язані з зонами безпеки, і можуть вплинути на те, як у центрі адміністрування Windows є користувачі Azure.</span><span class="sxs-lookup"><span data-stu-id="25afd-103">Microsoft Edge has [known issues](https://go.microsoft.com/fwlink/?linkid=2140608) that are related to security zones and might affect how Azure users log in to Windows Admin Center.</span></span> <span data-ttu-id="25afd-104">Якщо у вас виникли проблеми з використанням функцій Azure в Microsoft EDGE, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="25afd-104">If you're having trouble using Azure features with Microsoft Edge, try the following steps:</span></span>

1. <span data-ttu-id="25afd-105">У меню " **Пуск** " знайдіть пункт властивості **браузера** та виберіть його.</span><span class="sxs-lookup"><span data-stu-id="25afd-105">In the **Start** menu, search for **Internet Options** and select it.</span></span>
2. <span data-ttu-id="25afd-106">У діалоговому вікні **Властивості браузера** перейдіть на вкладку **Безпека** .</span><span class="sxs-lookup"><span data-stu-id="25afd-106">In the **Internet Properties** dialog box, go to the **Security** tab.</span></span>
3. <span data-ttu-id="25afd-107">Виберіть зону **надійних сайтів** , а потім натисніть кнопку **сайти** .</span><span class="sxs-lookup"><span data-stu-id="25afd-107">Select the **Trusted sites** zone and then select the **Sites** button.</span></span>
4. <span data-ttu-id="25afd-108">У діалоговому вікні **Надійні веб-сайти** додайте URL-адресу шлюзу, а також [https://login.microsoftonline.com](https://login.microsoftonline.com) , а [https://login.live.com](https://login.live.com) потім натисніть кнопку **закрити**.</span><span class="sxs-lookup"><span data-stu-id="25afd-108">In the **Trusted sites** dialog box, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
5. <span data-ttu-id="25afd-109">У діалоговому вікні **Властивості браузера** перейдіть на вкладку **конфіденційність** .</span><span class="sxs-lookup"><span data-stu-id="25afd-109">In the **Internet Properties** dialog box, go to the **Privacy** tab.</span></span>
6. <span data-ttu-id="25afd-110">У розділі **блокування спливаючих вікон** натисніть кнопку **настройки**.</span><span class="sxs-lookup"><span data-stu-id="25afd-110">In the **Pop-up Blocker** section, select **Settings**.</span></span> <span data-ttu-id="25afd-111">У діалоговому вікні, що Відкриється, додайте URL-адресу шлюзу, а [https://login.microsoftonline.com](https://login.microsoftonline.com) також [https://login.live.com](https://login.live.com) , а потім натисніть кнопку **закрити**.</span><span class="sxs-lookup"><span data-stu-id="25afd-111">In the dialog box that opens, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
