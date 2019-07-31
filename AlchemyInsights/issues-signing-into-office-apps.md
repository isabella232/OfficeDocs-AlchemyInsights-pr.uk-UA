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
- "2559"
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938384"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="77e2a-102">Фіксація Office apps "модуля TPM надійних ваш комп'ютер працює неправильно" повідомлення</span><span class="sxs-lookup"><span data-stu-id="77e2a-102">Fixing the Office apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="77e2a-103">Щоб виправити цю помилку, спробуйте наступне:</span><span class="sxs-lookup"><span data-stu-id="77e2a-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="77e2a-104">Інсталюйте останні оновлення для [Windows](https://support.microsoft.com/help/4027667/windows-10-update) і [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="77e2a-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="77e2a-105">[Ясно Office облікові дані](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) за допомогою диспетчера облікових даних Windows.</span><span class="sxs-lookup"><span data-stu-id="77e2a-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="77e2a-106">**Примітка:** 16,0 змінили реєстру доріжки для офісу 2016.</span><span class="sxs-lookup"><span data-stu-id="77e2a-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="77e2a-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="77e2a-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="77e2a-108">Повторіть [процес відновлення користувача](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) виправити надійні платформи модуля TPM невдач.</span><span class="sxs-lookup"><span data-stu-id="77e2a-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="77e2a-109">Встановити в EnableADAL = 0, виконавши наведені нижче дії:</span><span class="sxs-lookup"><span data-stu-id="77e2a-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="77e2a-110">Клацніть правою кнопкою миші кнопку Windows Пуск, виберіть **виконати**, введіть **regedit**а потім виберіть **ОК**.</span><span class="sxs-lookup"><span data-stu-id="77e2a-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="77e2a-111">Виберіть, **так** щоб дозволити редактор реєстру для внесення змін до пристрою.</span><span class="sxs-lookup"><span data-stu-id="77e2a-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="77e2a-112">У редакторі реєстру додайте значення DWORD з **EnableADAL** з значення **0** під HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="77e2a-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="77e2a-113">Докладніше перегляньте [підключення проблеми у входу після оновлення до Office 2016 побудувати 16.0.7967 на версії 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="77e2a-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>