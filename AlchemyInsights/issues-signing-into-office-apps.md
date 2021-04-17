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
- "2559"
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833036"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="7d9ef-102">Виправлення помилок у програмах Microsoft 365 "Модуль надійної платформи комп'ютера працює неправильно"</span><span class="sxs-lookup"><span data-stu-id="7d9ef-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="7d9ef-103">Щоб виправити цю помилку, спробуйте виконати наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="7d9ef-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="7d9ef-104">Інсталюйте останні оновлення [для Windows](https://support.microsoft.com/help/4027667/windows-10-update) і [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="7d9ef-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="7d9ef-105">[Видаліть облікові дані Office за](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) допомогою диспетчера облікових даних Windows.</span><span class="sxs-lookup"><span data-stu-id="7d9ef-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="7d9ef-106">**Примітка.** Шляхи реєстру для Пакета Office 2016 змінено на 16.0.</span><span class="sxs-lookup"><span data-stu-id="7d9ef-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="7d9ef-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="7d9ef-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="7d9ef-108">Спробуйте відновити [користувача, щоб](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) виправити помилки модуля TPM.</span><span class="sxs-lookup"><span data-stu-id="7d9ef-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="7d9ef-109">Установіть значення EnableADAL = 0, як описано нижче.</span><span class="sxs-lookup"><span data-stu-id="7d9ef-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="7d9ef-110">Клацніть правою кнопкою миші кнопку Пуск, виберіть **команду Виконати,** введіть **regedit** і натисніть кнопку **OK.**</span><span class="sxs-lookup"><span data-stu-id="7d9ef-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="7d9ef-111">Виберіть **Так,** щоб дозволити редактору реєстру вносити зміни на пристрої.</span><span class="sxs-lookup"><span data-stu-id="7d9ef-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="7d9ef-112">У редакторі реєстру додайте значення DWORD **параметра EnableADAL** із **значенням 0** у розділі HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="7d9ef-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="7d9ef-113">Докладні відомості див. в статтях Проблеми з підключенням після входу в систему після оновлення [до збірки Office 2016 16.0.7967 у Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)</span><span class="sxs-lookup"><span data-stu-id="7d9ef-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>