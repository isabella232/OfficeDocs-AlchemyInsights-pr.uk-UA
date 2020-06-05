---
title: Проблеми з входом у програми Microsoft 365
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
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579922"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="e105d-102">Порожній екран входу в Microsoft 365 Apps</span><span class="sxs-lookup"><span data-stu-id="e105d-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="e105d-103">Щоб вирішити цю проблему, спробуйте виконати такі дії:</span><span class="sxs-lookup"><span data-stu-id="e105d-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="e105d-104">Інсталюйте останні оновлення для [Windows](https://support.microsoft.com/help/4027667/windows-10-update) і [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="e105d-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="e105d-105">Скидання параметрів браузера Internet Explorer: перейдіть до розділу **засоби**  >  **Інтернет-параметри**  >  **Розширений**  >  **Скидання настройок браузера Internet Explorer** (Зауважте, що ви втратите користувацькі настройки), а потім спробуйте ввійти в Office знову.</span><span class="sxs-lookup"><span data-stu-id="e105d-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="e105d-106">Вимкніть захисник програми Windows Defender (WDAG) або будь-який подібний брандмауер або антивірусна програма:</span><span class="sxs-lookup"><span data-stu-id="e105d-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="e105d-107">На панелі керування перейдіть до **програми**, а потім виберіть пункт **Увімкнути або вимкнути засоби Windows**.</span><span class="sxs-lookup"><span data-stu-id="e105d-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="e105d-108">Якщо активовано програму захисту захисника Windows, спробуйте вимкнути його.</span><span class="sxs-lookup"><span data-stu-id="e105d-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="e105d-109">**Примітка:** Можливо, потрібно буде перезавантажити комп'ютер.</span><span class="sxs-lookup"><span data-stu-id="e105d-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="e105d-110">Переконайтеся, що Microsoft. сад. брокера [сад WAM Plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) не блокується будь-який додаток або брандмауер/антивірусна програма.</span><span class="sxs-lookup"><span data-stu-id="e105d-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="e105d-111">[Очистіть облікові дані Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) за допомогою диспетчера облікових даних Windows.</span><span class="sxs-lookup"><span data-stu-id="e105d-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="e105d-112">**Примітка:** Шлях до реєстру для Office 2016 змінено на 16,0.</span><span class="sxs-lookup"><span data-stu-id="e105d-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="e105d-113">(Напр.: \ програмне забезпеченя \mice\)</span><span class="sxs-lookup"><span data-stu-id="e105d-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="e105d-114">Щоб отримати додаткові відомості див [проблеми з підключенням після оновлення до Office 2016, створення 16.0.7967 на Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="e105d-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>