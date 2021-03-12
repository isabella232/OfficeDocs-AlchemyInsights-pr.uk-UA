---
title: Проблеми з входом в програми Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709127"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="ed691-102">Виправлення повідомлень програми Microsoft 365 "модуль надійної платформи на комп'ютері не функціонує</span><span class="sxs-lookup"><span data-stu-id="ed691-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="ed691-103">Щоб виправити цю помилку, спробуйте виконати наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="ed691-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="ed691-104">Інсталюйте найновіші оновлення для [Windows](https://support.microsoft.com/help/4027667/windows-10-update) і [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="ed691-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="ed691-105">[Очищення облікових даних Office](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) за допомогою диспетчера облікових даних Windows.</span><span class="sxs-lookup"><span data-stu-id="ed691-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="ed691-106">**Примітка.** Шляхи реєстру для Office 2016 змінилися на 16,0.</span><span class="sxs-lookup"><span data-stu-id="ed691-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="ed691-107">(Приклад: \Software\microsoft\office\16.0\coment\identity\)</span><span class="sxs-lookup"><span data-stu-id="ed691-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="ed691-108">Випробуйте [процес відновлення користувача](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) , щоб виправити помилки модуля TPM.</span><span class="sxs-lookup"><span data-stu-id="ed691-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="ed691-109">Установіть значення EnableADAL = 0, виконавши наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="ed691-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="ed691-110">Клацніть правою кнопкою миші кнопку Windows Пуск, виберіть команду **виконати**, введіть **Regedit** і натисніть **кнопку OK**.</span><span class="sxs-lookup"><span data-stu-id="ed691-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="ed691-111">Натисніть кнопку " **так** ", щоб дозволити редактору реєстру вносити зміни до вашого пристрою.</span><span class="sxs-lookup"><span data-stu-id="ed691-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="ed691-112">У редакторі реєстру додайте значення DWORD в **EnableADAL** з параметром **0** під HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="ed691-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="ed691-113">Щоб отримати докладніші відомості, ознайомтеся з [проблемами підключення під час входу в Office 2016 збірці 16.0.7967 у Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="ed691-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>