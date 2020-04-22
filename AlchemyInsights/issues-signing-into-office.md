---
title: Проблеми з входом у програми Office
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
ms.openlocfilehash: 695d449a876c22ff441da2367ef67aaea470eb66
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763022"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="088db-102">Проблеми з входом у програми Office</span><span class="sxs-lookup"><span data-stu-id="088db-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="088db-103">Щоб вирішити проблеми з входу в програмах Office, спробуйте виконати наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="088db-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="088db-104">Видалити всі робочі облікові записи, крім відповідного облікового запису, за допомогою настройок Windows > **доступ до роботи або школи**.</span><span class="sxs-lookup"><span data-stu-id="088db-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="088db-105">[Очистіть облікові дані Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) за допомогою диспетчера облікових даних Windows.</span><span class="sxs-lookup"><span data-stu-id="088db-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="088db-106">**Примітка:** Шлях до реєстру для Office 2016 змінено на 16,0.</span><span class="sxs-lookup"><span data-stu-id="088db-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="088db-107">(Напр.: \ програмне забезпеченя \mice\)</span><span class="sxs-lookup"><span data-stu-id="088db-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="088db-108">Відкрийте програму Office **, виберіть** > **обліковий запис** > для**входу**. Ввійдіть за допомогою облікового запису користувача з дійсною ліцензією.</span><span class="sxs-lookup"><span data-stu-id="088db-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="088db-109">Докладні відомості див. в статті [Облікові записи в Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="088db-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="088db-110">Для Mac див. статтю [Не вдається ввійти в програму Office 2016 для Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="088db-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="088db-111">Якщо виникає помилка під час підключення до Microsoft 365 за допомогою Office 2013, увімкніть сучасних автентифікації для Office клієнта.</span><span class="sxs-lookup"><span data-stu-id="088db-111">If the errors occurs while connecting to Microsoft 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="088db-112">Докладні відомості див. у статтях:</span><span class="sxs-lookup"><span data-stu-id="088db-112">For more information, see:</span></span>
- [<span data-ttu-id="088db-113">Не вдається ввійти до Microsoft 365, Azure або InTune</span><span class="sxs-lookup"><span data-stu-id="088db-113">You can't sign in to Microsoft 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="088db-114">Проблеми з підключенням у входу після оновлення до Office 2016, створення 16.0.7967 на Windows 10</span><span class="sxs-lookup"><span data-stu-id="088db-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="088db-115">"На жаль, інший обліковий запис з вашої організації вже ввійшли до цього комп'ютера" в Office</span><span class="sxs-lookup"><span data-stu-id="088db-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="088db-116">Усунення проблем із входу з Office, сучасна Автентифікація під час використання ADFS</span><span class="sxs-lookup"><span data-stu-id="088db-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)