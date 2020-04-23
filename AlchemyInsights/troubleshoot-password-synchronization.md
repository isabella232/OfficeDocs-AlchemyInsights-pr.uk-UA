---
title: Виправлення неполадок синхронізації паролів
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732531"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="85fee-102">Виправлення неполадок синхронізації паролів</span><span class="sxs-lookup"><span data-stu-id="85fee-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="85fee-103">Щоб вирішити проблеми, де немає паролів синхронізується з Azure AD-підключення версії 1.1.614.0 або пізнішої:</span><span class="sxs-lookup"><span data-stu-id="85fee-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="85fee-104">Відкрийте новий сеанс Windows PowerShell на сервері Azure AD-підключення, за допомогою параметра запуск із правами **адміністратора** .</span><span class="sxs-lookup"><span data-stu-id="85fee-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="85fee-105">Запустіть **Set-виконання політики, Пульс,** або **набір-виконання політики необмежений**.</span><span class="sxs-lookup"><span data-stu-id="85fee-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span>

3. <span data-ttu-id="85fee-106">Запустіть майстер Azure AD-підключення.</span><span class="sxs-lookup"><span data-stu-id="85fee-106">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="85fee-107">Перейдіть до сторінки **додаткові завдання** , виберіть **Виправлення неполадок**і натисніть кнопку **Далі**.</span><span class="sxs-lookup"><span data-stu-id="85fee-107">Navigate to the **Additional Tasks** page, select **Troubleshoot**, and click **Next**.</span></span>

5. <span data-ttu-id="85fee-108">На сторінці виправлення неполадок натисніть кнопку **Запуск, щоб запустити меню виправлення неполадок** у PowerShell.</span><span class="sxs-lookup"><span data-stu-id="85fee-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span>

6. <span data-ttu-id="85fee-109">У головному меню виберіть пункт **Виправлення неполадок синхронізації паролів**.</span><span class="sxs-lookup"><span data-stu-id="85fee-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span>

7. <span data-ttu-id="85fee-110">У підменю виберіть **синхронізація пароля не працює взагалі**.</span><span class="sxs-lookup"><span data-stu-id="85fee-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span>

<span data-ttu-id="85fee-111">**Зрозуміти результати завдання з виправлення неполадок**</span><span class="sxs-lookup"><span data-stu-id="85fee-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="85fee-112">Завдання виправлення неполадок, виконує такі перевірки:</span><span class="sxs-lookup"><span data-stu-id="85fee-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="85fee-113">Перевіряє, чи активовано функцію синхронізації паролів для клієнта Azure AD.</span><span class="sxs-lookup"><span data-stu-id="85fee-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>

- <span data-ttu-id="85fee-114">Перевіряє, чи сервер Azure AD-підключення не в режимі проміжного.</span><span class="sxs-lookup"><span data-stu-id="85fee-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>

- <span data-ttu-id="85fee-115">Для кожного наявного локального з'єднувача Active Directory (який відповідає наявному лісі Active Directory):</span><span class="sxs-lookup"><span data-stu-id="85fee-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>

- 
  - <span data-ttu-id="85fee-116">Перевіряє, чи ввімкнуто функцію синхронізація пароля.</span><span class="sxs-lookup"><span data-stu-id="85fee-116">Validates that the password synchronization feature is enabled.</span></span>

  - <span data-ttu-id="85fee-117">Пошук для синхронізації пароля серцебиття події в журналах подій застосунків Windows.</span><span class="sxs-lookup"><span data-stu-id="85fee-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>

  - <span data-ttu-id="85fee-118">Для кожного домену Active Directory, у розділі локальної служби Active Directory-з'єднувач:</span><span class="sxs-lookup"><span data-stu-id="85fee-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>

  - <span data-ttu-id="85fee-119">Перевіряє, що домен, доступний із сервера Azure AD-підключення.</span><span class="sxs-lookup"><span data-stu-id="85fee-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>

  - <span data-ttu-id="85fee-120">Перевіряє, чи облікові записи служби доменів Active Directory (AD DS), які використовуються на локальному з'єднувачі Active Directory, має правильні ім'я користувача, пароль і дозволи, потрібні для синхронізації паролів.</span><span class="sxs-lookup"><span data-stu-id="85fee-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>

<span data-ttu-id="85fee-121">Щоб дізнатися більше про виправлення неполадок пароль синхронізації [, див.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization)</span><span class="sxs-lookup"><span data-stu-id="85fee-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  