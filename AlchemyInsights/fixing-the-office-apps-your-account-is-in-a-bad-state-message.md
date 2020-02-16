---
title: Фіксація програм Office обліковий запис перебуває в повідомленні поганий стан
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969913"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="3266d-102">Виправлення помилок програм Office "ваш обліковий запис перебуває в поганому стані"</span><span class="sxs-lookup"><span data-stu-id="3266d-102">Fixing the Office apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="3266d-103">Щоб виправити цю помилку, спробуйте на проблемному комп'ютері такі параметри:</span><span class="sxs-lookup"><span data-stu-id="3266d-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="3266d-104">Відкрийте програму Office **, виберіть** > **обліковий запис** > ,**вийдіть із всіх облікових записів**.</span><span class="sxs-lookup"><span data-stu-id="3266d-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="3266d-105">Увійдіть знову, використовуючи обліковий запис користувача з дійсною ліцензією.</span><span class="sxs-lookup"><span data-stu-id="3266d-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="3266d-106">Докладні відомості наведено [в облікових записах в Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="3266d-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="3266d-107">[Очистіть облікові дані Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) за допомогою диспетчера облікових даних Windows.</span><span class="sxs-lookup"><span data-stu-id="3266d-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="3266d-108">**Примітка:** Шлях до реєстру для Office 2016 змінено на 16,0.</span><span class="sxs-lookup"><span data-stu-id="3266d-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="3266d-109">Наприклад, \ програмне Забезпечена\micfr\fore\16.0\ \ \ </span><span class="sxs-lookup"><span data-stu-id="3266d-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="3266d-110">На проблемному комп'ютері встановіть EnableADAL = 0, виконавши такі дії:</span><span class="sxs-lookup"><span data-stu-id="3266d-110">On the affected computer, set the EnableADAL = 0 using the following steps:</span></span>  
     1. <span data-ttu-id="3266d-111">Клацніть правою кнопкою миші кнопку Windows і виберіть **запустити**.</span><span class="sxs-lookup"><span data-stu-id="3266d-111">Right-click the Windows button and select **Run**.</span></span> <span data-ttu-id="3266d-112">У полі " **Відкрити** " введіть **Regedit**і виберіть **"OK"**.</span><span class="sxs-lookup"><span data-stu-id="3266d-112">In the **Open** box, type **regedit**, and then select **OK**.</span></span>
     2. <span data-ttu-id="3266d-113">Виберіть **так** , коли буде запропоновано дозволити редактору реєстру вносити зміни до пристрою.</span><span class="sxs-lookup"><span data-stu-id="3266d-113">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="3266d-114">У редакторі реєстру, додайте значення DWORD з EnableADAL параметр 0, у розділі HKEY_CURRENT_USER \ програмне Забезпеченми\mice\foot\16.0\ind\idt.</span><span class="sxs-lookup"><span data-stu-id="3266d-114">In the Registry Editor, add a DWORD value of EnableADAL with a setting of 0 under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>
- <span data-ttu-id="3266d-115">Якщо сталася помилка під час підключення до Office 365 за допомогою Office 2013, [Увімкніть сучасних автентифікації](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) для клієнта Office.</span><span class="sxs-lookup"><span data-stu-id="3266d-115">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="3266d-116">Щоб отримати додаткові відомості, Дізнайтеся, [як вирішити проблеми, не-браузер застосунків, які не вдається ввійти до Office 365, Azure або InTune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span><span class="sxs-lookup"><span data-stu-id="3266d-116">For more information, see [How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

