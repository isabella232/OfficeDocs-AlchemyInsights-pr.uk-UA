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
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579886"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="98fac-102">Виправлення програми Microsoft 365, "довірений платформи модуль не функціонує належним чином" повідомлення</span><span class="sxs-lookup"><span data-stu-id="98fac-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="98fac-103">Щоб виправити цю помилку, спробуйте виконати наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="98fac-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="98fac-104">Інсталюйте останні оновлення для [Windows](https://support.microsoft.com/help/4027667/windows-10-update) і [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="98fac-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="98fac-105">[Очистіть облікові дані Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) за допомогою диспетчера облікових даних Windows.</span><span class="sxs-lookup"><span data-stu-id="98fac-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="98fac-106">**Примітка:** Шлях до реєстру для Office 2016 змінено на 16,0.</span><span class="sxs-lookup"><span data-stu-id="98fac-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="98fac-107">(Напр.: \ програмне забезпеченя \mice\)</span><span class="sxs-lookup"><span data-stu-id="98fac-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="98fac-108">Спробуйте [процес відновлення користувача](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) , щоб виправити НЕПОЛАДКИ модуля TPM.</span><span class="sxs-lookup"><span data-stu-id="98fac-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="98fac-109">Встановіть EnableADAL = 0, виконавши наступні кроки:</span><span class="sxs-lookup"><span data-stu-id="98fac-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="98fac-110">Клацніть правою кнопкою миші кнопку Пуск Windows, виберіть **запустити**, введіть **Regedit**і натисніть кнопку **OK**.</span><span class="sxs-lookup"><span data-stu-id="98fac-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="98fac-111">Виберіть **так** , щоб дозволити редактору реєстру вносити зміни до пристрою.</span><span class="sxs-lookup"><span data-stu-id="98fac-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="98fac-112">У редакторі реєстру, додайте значення DWORD з **EnableADAL** параметр **0** , у розділі HKEY_CURRENT_USER \ програмне Забезпечена\mice\foot\16.0\ind\idat.</span><span class="sxs-lookup"><span data-stu-id="98fac-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="98fac-113">Щоб отримати додаткові відомості див [проблеми з підключенням після оновлення до Office 2016, створення 16.0.7967 на Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="98fac-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>