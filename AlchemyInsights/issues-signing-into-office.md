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
- "2574"
ms.openlocfilehash: 3622a3408b25b43090e9414ae5ffcfc2760264ee
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938382"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="c54cf-102">Питання, ввійшовши до служби Office</span><span class="sxs-lookup"><span data-stu-id="c54cf-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="c54cf-103">Для усунення проблем входу з Office apps, спробуйте наступне:</span><span class="sxs-lookup"><span data-stu-id="c54cf-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="c54cf-104">Видалити всі роботи облікових записів, за винятком постраждалих облікового запису, використовуючи настройки Windows > **доступу роботу або в школі**.</span><span class="sxs-lookup"><span data-stu-id="c54cf-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="c54cf-105">[Ясно Office облікові дані](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) за допомогою диспетчера облікових даних Windows.</span><span class="sxs-lookup"><span data-stu-id="c54cf-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="c54cf-106">**Примітка:** 16,0 змінили реєстру доріжки для офісу 2016.</span><span class="sxs-lookup"><span data-stu-id="c54cf-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="c54cf-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="c54cf-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="c54cf-108">Відкрийте застосунок Office, виберіть " **файл**" > **рахунок** > **Вихід**. Потім увійдіть за допомогою облікового запису користувача з діючою ліцензією.</span><span class="sxs-lookup"><span data-stu-id="c54cf-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="c54cf-109">Докладну інформацію переглянути [облікові записи в офісі](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="c54cf-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="c54cf-110">Для Mac див [не вдається ввійти в офісі 2016 для Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="c54cf-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="c54cf-111">Якщо помилки виникає під час підключення до Office 365, за допомогою Office 2013, увімкніть сучасних автентифікації для офісу клієнта.</span><span class="sxs-lookup"><span data-stu-id="c54cf-111">If the errors occurs while connecting to Office 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="c54cf-112">у перелічених нижче статтях.</span><span class="sxs-lookup"><span data-stu-id="c54cf-112">For more information, see:</span></span>
- [<span data-ttu-id="c54cf-113">Ви не можете ввійти до Office 365, Azure або Intune</span><span class="sxs-lookup"><span data-stu-id="c54cf-113">You can't sign in to Office 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="c54cf-114">Підключення проблеми у входу після оновлення до Office 2016 побудувати 16.0.7967 на версії 10</span><span class="sxs-lookup"><span data-stu-id="c54cf-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="c54cf-115">"На жаль, інший обліковий запис з вашої організації вже ввійшли до цього комп'ютера" в офісі</span><span class="sxs-lookup"><span data-stu-id="c54cf-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="c54cf-116">Неполадки входу з автентифікацією сучасні офісні під час використання ADFS</span><span class="sxs-lookup"><span data-stu-id="c54cf-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)