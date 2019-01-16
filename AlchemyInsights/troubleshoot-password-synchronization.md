---
title: 'Усунення проблем: синхронізація пароля'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: c71fce8621057093d23891c26f7b0285fdc8b9ed
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/15/2019
ms.locfileid: "28319517"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="12363-102">Усунення проблем: синхронізація пароля</span><span class="sxs-lookup"><span data-stu-id="12363-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="12363-103">Для виправлення неполадок, де немає паролі синхронізовані з Azure оголошення підключення версії 1.1.614.0 або пізнішої версії:</span><span class="sxs-lookup"><span data-stu-id="12363-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="12363-104">Відкриття сеансу новий Windows PowerShell Azure оголошення підключення сервера з можливість **запускати з правами адміністратора** .</span><span class="sxs-lookup"><span data-stu-id="12363-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span> 
    
2. <span data-ttu-id="12363-105">Запустити **набір-політику виконання RemoteSigned** або **набір-політику виконання необмежений**.</span><span class="sxs-lookup"><span data-stu-id="12363-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span> 
    
3. <span data-ttu-id="12363-106">Запустіть майстер Azure оголошення підключитися.</span><span class="sxs-lookup"><span data-stu-id="12363-106">Start the Azure AD Connect wizard.</span></span>
    
4. <span data-ttu-id="12363-107">Перейдіть до на \* \* додаткові завдання \* \* сторінки, виберіть \* \* виправлення неполадок \* \* і натисніть кнопку **Далі**.</span><span class="sxs-lookup"><span data-stu-id="12363-107">Navigate to the \*\* Additional Tasks \*\* page, select \*\* Troubleshoot \*\*, and click **Next**.</span></span> 
    
5. <span data-ttu-id="12363-108">На сторінці виправлення неполадок **запуску почати усуненням неполадок** у натисніть меню PowerShell.</span><span class="sxs-lookup"><span data-stu-id="12363-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span> 
    
6. <span data-ttu-id="12363-109">У головному меню виберіть **Виправити неполадки синхронізації паролів**.</span><span class="sxs-lookup"><span data-stu-id="12363-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span> 
    
7. <span data-ttu-id="12363-110">У меню Південь» виберіть **пароль працює на всіх**.</span><span class="sxs-lookup"><span data-stu-id="12363-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span> 
    
 <span data-ttu-id="12363-111">**Оцінити результати виправлення неполадок завдання**</span><span class="sxs-lookup"><span data-stu-id="12363-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="12363-112">Виправлення неполадок завдання виконує такі перевірки:</span><span class="sxs-lookup"><span data-stu-id="12363-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="12363-113">Перевіряє ввімкнутий функцію синхронізації паролів для блакитні оголошення орендаря.</span><span class="sxs-lookup"><span data-stu-id="12363-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>
    
- <span data-ttu-id="12363-114">Підтверджує, що Azure оголошення підключення сервера немає в постановці режимі.</span><span class="sxs-lookup"><span data-stu-id="12363-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>
    
- <span data-ttu-id="12363-115">Для кожного наявної локальної служби Active Directory connector (що відповідає для існуючі лісу Active Directory):</span><span class="sxs-lookup"><span data-stu-id="12363-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>
    
- 
  - <span data-ttu-id="12363-116">Підтверджує, що увімкнуто функцію синхронізації паролів.</span><span class="sxs-lookup"><span data-stu-id="12363-116">Validates that the password synchronization feature is enabled.</span></span>
    
  - <span data-ttu-id="12363-117">Шукає пароль синхронізації серцебиття події журналу подій Windows додатків.</span><span class="sxs-lookup"><span data-stu-id="12363-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>
    
  - <span data-ttu-id="12363-118">Для кожного домену Active Directory, у розділі Локальні Active Directory connector:</span><span class="sxs-lookup"><span data-stu-id="12363-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>
    
  - <span data-ttu-id="12363-119">Підтверджує, що домен можна дістатися з Azure оголошення підключення сервера.</span><span class="sxs-lookup"><span data-stu-id="12363-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>
    
  - <span data-ttu-id="12363-120">Підтверджує, що облікові записи служб домену Active Directory (AD DS), що використовуються локальні Active Directory connector має правильне ім'я користувача, пароль і дозволів, потрібних для синхронізації паролів.</span><span class="sxs-lookup"><span data-stu-id="12363-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>
    
<span data-ttu-id="12363-121">За допомогою виправлення неполадок синхронізації паролів див. [Виправлення неполадок синхронізація пароля з Azure оголошення підключення синхронізації](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="12363-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  

