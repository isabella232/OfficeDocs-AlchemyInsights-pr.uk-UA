---
title: 'Усунення проблем: синхронізація пароля'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: d346cf97fb2fd08a9132904517192d8728ffa941
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29924717"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="07622-102">Усунення проблем: синхронізація пароля</span><span class="sxs-lookup"><span data-stu-id="07622-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="07622-103">Для виправлення неполадок, де немає паролі синхронізовані з Azure оголошення підключення версії 1.1.614.0 або пізнішої версії:</span><span class="sxs-lookup"><span data-stu-id="07622-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="07622-104">Відкриття сеансу новий Windows PowerShell Azure оголошення підключення сервера з можливість **запускати з правами адміністратора** .</span><span class="sxs-lookup"><span data-stu-id="07622-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span> 
    
2. <span data-ttu-id="07622-105">Запустити **набір-політику виконання RemoteSigned** або **набір-політику виконання необмежений**.</span><span class="sxs-lookup"><span data-stu-id="07622-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span> 
    
3. <span data-ttu-id="07622-106">Запустіть майстер Azure оголошення підключитися.</span><span class="sxs-lookup"><span data-stu-id="07622-106">Start the Azure AD Connect wizard.</span></span>
    
4. <span data-ttu-id="07622-107">Перейдіть до на \* \* додаткові завдання \* \* сторінки, виберіть \* \* виправлення неполадок \* \* і натисніть кнопку **Далі**.</span><span class="sxs-lookup"><span data-stu-id="07622-107">Navigate to the \*\* Additional Tasks \*\* page, select \*\* Troubleshoot \*\*, and click **Next**.</span></span> 
    
5. <span data-ttu-id="07622-108">На сторінці виправлення неполадок **запуску почати усуненням неполадок** у натисніть меню PowerShell.</span><span class="sxs-lookup"><span data-stu-id="07622-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span> 
    
6. <span data-ttu-id="07622-109">У головному меню виберіть **Виправити неполадки синхронізації паролів**.</span><span class="sxs-lookup"><span data-stu-id="07622-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span> 
    
7. <span data-ttu-id="07622-110">У меню Південь» виберіть **пароль працює на всіх**.</span><span class="sxs-lookup"><span data-stu-id="07622-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span> 
    
 <span data-ttu-id="07622-111">**Оцінити результати виправлення неполадок завдання**</span><span class="sxs-lookup"><span data-stu-id="07622-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="07622-112">Виправлення неполадок завдання виконує такі перевірки:</span><span class="sxs-lookup"><span data-stu-id="07622-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="07622-113">Перевіряє ввімкнутий функцію синхронізації паролів для блакитні оголошення орендаря.</span><span class="sxs-lookup"><span data-stu-id="07622-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>
    
- <span data-ttu-id="07622-114">Підтверджує, що Azure оголошення підключення сервера немає в постановці режимі.</span><span class="sxs-lookup"><span data-stu-id="07622-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>
    
- <span data-ttu-id="07622-115">Для кожного наявної локальної служби Active Directory connector (що відповідає для існуючі лісу Active Directory):</span><span class="sxs-lookup"><span data-stu-id="07622-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>
    
- 
  - <span data-ttu-id="07622-116">Підтверджує, що увімкнуто функцію синхронізації паролів.</span><span class="sxs-lookup"><span data-stu-id="07622-116">Validates that the password synchronization feature is enabled.</span></span>
    
  - <span data-ttu-id="07622-117">Шукає пароль синхронізації серцебиття події журналу подій Windows додатків.</span><span class="sxs-lookup"><span data-stu-id="07622-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>
    
  - <span data-ttu-id="07622-118">Для кожного домену Active Directory, у розділі Локальні Active Directory connector:</span><span class="sxs-lookup"><span data-stu-id="07622-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>
    
  - <span data-ttu-id="07622-119">Підтверджує, що домен можна дістатися з Azure оголошення підключення сервера.</span><span class="sxs-lookup"><span data-stu-id="07622-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>
    
  - <span data-ttu-id="07622-120">Підтверджує, що облікові записи служб домену Active Directory (AD DS), що використовуються локальні Active Directory connector має правильне ім'я користувача, пароль і дозволів, потрібних для синхронізації паролів.</span><span class="sxs-lookup"><span data-stu-id="07622-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>
    
<span data-ttu-id="07622-121">За допомогою виправлення неполадок синхронізації паролів див. [Виправлення неполадок синхронізація пароля з Azure оголошення підключення синхронізації](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="07622-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  

