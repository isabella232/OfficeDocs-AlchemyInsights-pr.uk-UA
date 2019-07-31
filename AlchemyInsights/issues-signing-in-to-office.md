---
title: Питання, ввійшовши до служби Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938383"
---
# <a name="blank-sign-in-screen-in-office-apps"></a><span data-ttu-id="df064-102">Пустий екрана входу в Office apps</span><span class="sxs-lookup"><span data-stu-id="df064-102">Blank sign-in screen in Office apps</span></span>

<span data-ttu-id="df064-103">Щоб виправити цю проблему, спробуйте наступне:</span><span class="sxs-lookup"><span data-stu-id="df064-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="df064-104">Інсталюйте останні оновлення для [Windows](https://support.microsoft.com/help/4027667/windows-10-update) і [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="df064-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="df064-105">Скинути параметри Internet Explorer: Заходимо **інструменти** > **Властивості браузера** > **Додатково** > **Скидання настройок Internet Explorer** (Зверніть увагу, що вам буде втрачено користувацькі настройки) після чого спробуйте ввійти до офісу знову.</span><span class="sxs-lookup"><span data-stu-id="df064-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="df064-106">Відключити будь-які аналогічні брандмауера або антивірусної програми або гвардії застосунок Windows Defender (WDAG):</span><span class="sxs-lookup"><span data-stu-id="df064-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="df064-107">На панелі керування перейдіть до **програми**а потім виберіть **засоби Windows увімкнути або вимкнути**.</span><span class="sxs-lookup"><span data-stu-id="df064-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="df064-108">Якщо активовано Windows Defender застосування гвардії, відключіть його.</span><span class="sxs-lookup"><span data-stu-id="df064-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="df064-109">**Примітка:** Може знадобитися перезавантаження комп'ютера.</span><span class="sxs-lookup"><span data-stu-id="df064-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="df064-110">Переконайтеся, що Microsoft.AAD.BrokerPlugin [Сад WAM плагін](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) не час заблоковано всі програми або брандмауер/anti-virus програми.</span><span class="sxs-lookup"><span data-stu-id="df064-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="df064-111">[Ясно Office облікові дані](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) за допомогою диспетчера облікових даних Windows.</span><span class="sxs-lookup"><span data-stu-id="df064-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="df064-112">**Примітка:** 16,0 змінили реєстру доріжки для офісу 2016.</span><span class="sxs-lookup"><span data-stu-id="df064-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="df064-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="df064-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="df064-114">Докладніше перегляньте [підключення проблеми у входу після оновлення до Office 2016 побудувати 16.0.7967 на версії 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="df064-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>