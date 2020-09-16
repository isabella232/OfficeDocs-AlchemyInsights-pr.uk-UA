---
title: Політики збереження в центрі адміністрування Exchange не працюють
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740531"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="11fb5-102">Політики збереження в центрі адміністрування Exchange</span><span class="sxs-lookup"><span data-stu-id="11fb5-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="11fb5-103">Якщо ви хочете, щоб ми могли виконати автоматичні перевірки для наведених нижче параметрів, натисніть кнопку назад, < – угорі цієї сторінки, а потім введіть адресу електронної пошти користувача, який має проблеми з політиками збереження.</span><span class="sxs-lookup"><span data-stu-id="11fb5-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="11fb5-104">**Проблема:** Щойно створені або оновлені політики збереження в центрі адміністрування Exchange не застосовуються до поштових скриньок або елементи, не переміщуються до архівної поштової скриньки або видаляються.</span><span class="sxs-lookup"><span data-stu-id="11fb5-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="11fb5-105">**Причини кореневої:**</span><span class="sxs-lookup"><span data-stu-id="11fb5-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="11fb5-106">Можливо, це пояснюється тим, що **помічник керованої папки** не обробляється поштовою скринькою користувача.</span><span class="sxs-lookup"><span data-stu-id="11fb5-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="11fb5-107">Помічник із керованих папок намагається виконати обробку кожної поштової скриньки в організації, що базується на хмарі, кожні сім днів.</span><span class="sxs-lookup"><span data-stu-id="11fb5-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="11fb5-108">Якщо змінити тег збереження або застосувати іншу політику збереження до поштової скриньки, можна зачекати, доки керована папка допоможе обробити поштову скриньку або запустити командлет Start-ManagedFolderAssistant, щоб запустити помічник із керованих папок для обробки певної поштової скриньки.</span><span class="sxs-lookup"><span data-stu-id="11fb5-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="11fb5-109">Запуск цього командлета стане в нагоді для тестування та виправлення неполадок політики збереження або параметрів тега збереження.</span><span class="sxs-lookup"><span data-stu-id="11fb5-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="11fb5-110">Щоб отримати докладніші відомості, перейдіть на вкладку [Запуск помічника з керованих папок](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="11fb5-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="11fb5-111">**Рішення:** Щоб запустити помічник із керованих папок для певної поштової скриньки, виконайте таку команду:</span><span class="sxs-lookup"><span data-stu-id="11fb5-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="11fb5-112">Це також може виникати, якщо в поштовій скриньці **ввімкнуто функцію** **Reensionhold** .</span><span class="sxs-lookup"><span data-stu-id="11fb5-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="11fb5-113">Якщо поштова скринька була розміщена на веб-сторінці, у цьому часі політику збереження в поштовій скриньці не буде оброблено.</span><span class="sxs-lookup"><span data-stu-id="11fb5-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="11fb5-114">Для отримання додаткових відомостей про настроювання в розділі Reensionhold: [утримання збереження поштової скриньки](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="11fb5-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="11fb5-115">**Рішення**</span><span class="sxs-lookup"><span data-stu-id="11fb5-115">**Solution:**</span></span>
    
  - <span data-ttu-id="11fb5-116">Перевірте стан параметра "повторна перевірка" на певній поштовій скриньці в [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="11fb5-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="11fb5-117">Виконайте таку команду, щоб **вимкнути функцію** reensionhold для певної поштової скриньки:</span><span class="sxs-lookup"><span data-stu-id="11fb5-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="11fb5-118">Тепер повторно запустіть Помічник із керованих папок:</span><span class="sxs-lookup"><span data-stu-id="11fb5-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="11fb5-119">**Примітка.** Якщо поштова скринька менше 10 МБ, помічник із керованих папок автоматично обробляє поштову скриньку.</span><span class="sxs-lookup"><span data-stu-id="11fb5-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="11fb5-120">Докладні відомості про політики збереження в центрі адміністрування Exchange наведено в статті:</span><span class="sxs-lookup"><span data-stu-id="11fb5-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="11fb5-121">Позначки збереження та політики збереження</span><span class="sxs-lookup"><span data-stu-id="11fb5-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="11fb5-122">Використання політики збереження в поштових скриньках</span><span class="sxs-lookup"><span data-stu-id="11fb5-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="11fb5-123">Додавання та видалення тегів збереження</span><span class="sxs-lookup"><span data-stu-id="11fb5-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="11fb5-124">Визначення типу утримання, розміщеного в поштовій скриньці</span><span class="sxs-lookup"><span data-stu-id="11fb5-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
