---
title: Проблеми з входом у програми Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833060"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="b4a99-102">Пустий екран входу в програмах Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="b4a99-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="b4a99-103">Щоб вирішити цю проблему, спробуйте зробити ось що:</span><span class="sxs-lookup"><span data-stu-id="b4a99-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="b4a99-104">Інсталюйте останні оновлення [для Windows](https://support.microsoft.com/help/4027667/windows-10-update) і [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="b4a99-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="b4a99-105">Скидання параметрів Internet Explorer: перейдіть до меню Знаряддя Властивості браузера Додаткові параметри скидання  >    >    >  **настройок Internet Explorer** (зверніть увагу, що ви втратите власні настройки), а потім спробуйте ввійти в Office ще раз.</span><span class="sxs-lookup"><span data-stu-id="b4a99-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="b4a99-106">Вимкніть Засіб захисту програм для Захисника Windows (WDAG) або будь-який подібний брандмауер чи антивірусну програму:</span><span class="sxs-lookup"><span data-stu-id="b4a99-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="b4a99-107">На Панелі керування відкрийте меню **Програми**, а потім виберіть елемент **Увімкнути або вимкнути компоненти Windows**.</span><span class="sxs-lookup"><span data-stu-id="b4a99-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="b4a99-108">Якщо засіб захисту програм для Захисника Windows увімкнуто, спробуйте вимкнути його.</span><span class="sxs-lookup"><span data-stu-id="b4a99-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="b4a99-109">**Примітка.** Можливо, знадобиться перезавантажити комп'ютер.</span><span class="sxs-lookup"><span data-stu-id="b4a99-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="b4a99-110">Переконайтеся, що компонент plug-in AAD.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) не блокується жодною програмою, брандмауером або антивірусним програмою.</span><span class="sxs-lookup"><span data-stu-id="b4a99-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="b4a99-111">[Видаліть облікові дані Office за](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) допомогою диспетчера облікових даних Windows.</span><span class="sxs-lookup"><span data-stu-id="b4a99-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="b4a99-112">**Примітка.** Шляхи реєстру для Пакета Office 2016 змінено на 16.0.</span><span class="sxs-lookup"><span data-stu-id="b4a99-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="b4a99-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="b4a99-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="b4a99-114">Докладні відомості див. в статтях Проблеми з підключенням після входу в систему після оновлення [до збірки Office 2016 16.0.7967 у Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)</span><span class="sxs-lookup"><span data-stu-id="b4a99-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>