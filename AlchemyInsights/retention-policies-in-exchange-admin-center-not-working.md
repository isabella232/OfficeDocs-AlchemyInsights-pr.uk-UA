---
title: Політики збереження в Центр адміністрування Exchange, не працює
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 4d3ca121c8d22a0900f136f7f2a754dfb5b435f5
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522828"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="75d7c-102">Політики збереження в Центр адміністрування Exchange</span><span class="sxs-lookup"><span data-stu-id="75d7c-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="75d7c-103">Якщо ви хочете, щоб запустити автоматизовані перевірки для наведених нижче параметрів, натисніть кнопку назад <--у верхній частині цієї сторінки, а потім введіть адресу електронної пошти користувача, який має проблеми з політики збереження.</span><span class="sxs-lookup"><span data-stu-id="75d7c-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="75d7c-104">**Проблема:** Створений або оновлений політики збереження в Центр адміністрування Exchange не застосовуються до поштових скриньок або елементи не переміщуються до поштової скриньки архіву або видалено.</span><span class="sxs-lookup"><span data-stu-id="75d7c-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="75d7c-105">**Кореневі причини:**</span><span class="sxs-lookup"><span data-stu-id="75d7c-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="75d7c-106">Можливо, **помічник із керованих папок** не обробляв поштову скриньку користувача.</span><span class="sxs-lookup"><span data-stu-id="75d7c-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="75d7c-107">Помічник із керованих папок намагається обробити кожну поштову скриньку в організації, розміщеній у хмарі, кожні сім днів.</span><span class="sxs-lookup"><span data-stu-id="75d7c-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="75d7c-108">Якщо змінити тег збереження або застосувати іншу політику збереження до поштової скриньки, можна зачекати, доки керовану папку допоможе обробити поштову скриньку, або запустити командлет Start-керовану помічника, щоб запустити помічник із керованих папок для обробки певної поштової скриньки.</span><span class="sxs-lookup"><span data-stu-id="75d7c-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="75d7c-109">Запуск цього командлета корисний для тестування або виправлення неполадок параметрів політики збереження або тегів збереження.</span><span class="sxs-lookup"><span data-stu-id="75d7c-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="75d7c-110">Для отримання додаткових відомостей відвідайте [запустіть Помічник із керованих папок](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="75d7c-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="75d7c-111">**Рішення:** Запустіть таку команду, щоб запустити помічник із керованих папок для певної поштової скриньки:</span><span class="sxs-lookup"><span data-stu-id="75d7c-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="75d7c-112">Це також може статися, якщо на поштову скриньку **увімкнуто** **Retentionhold** .</span><span class="sxs-lookup"><span data-stu-id="75d7c-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="75d7c-113">Якщо поштову скриньку було розміщено на RetentionHold, політика збереження поштової скриньки не оброблятиметься протягом цього часу.</span><span class="sxs-lookup"><span data-stu-id="75d7c-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="75d7c-114">Для отримання додаткових параметрів на RetentionHold параметр відображається: [утримання збереження поштової скриньки](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="75d7c-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="75d7c-115">**Рішення:**</span><span class="sxs-lookup"><span data-stu-id="75d7c-115">**Solution:**</span></span>
    
  - <span data-ttu-id="75d7c-116">Перевірте стан RetentionHold налаштування на конкретну поштову скриньку в [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="75d7c-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="75d7c-117">Запустіть таку команду, щоб **Вимкнути** retentionhold на конкретну поштову скриньку:</span><span class="sxs-lookup"><span data-stu-id="75d7c-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="75d7c-118">Тепер знову запустіть Помічник із керованих папок:</span><span class="sxs-lookup"><span data-stu-id="75d7c-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="75d7c-119">**Примітка:** Якщо поштова скринька менше 10 МБ, помічник із керованих папок не буде автоматично обробляти поштову скриньку.</span><span class="sxs-lookup"><span data-stu-id="75d7c-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="75d7c-120">Щоб отримати додаткові відомості про політики збереження в Центр адміністрування Exchange див.:</span><span class="sxs-lookup"><span data-stu-id="75d7c-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="75d7c-121">Теги збереження та політики збереження</span><span class="sxs-lookup"><span data-stu-id="75d7c-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="75d7c-122">Застосування політики збереження до поштових скриньок</span><span class="sxs-lookup"><span data-stu-id="75d7c-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="75d7c-123">Додавання або видалення тегів збереження</span><span class="sxs-lookup"><span data-stu-id="75d7c-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="75d7c-124">Як визначити тип утримання, розміщеного на поштовій скриньці</span><span class="sxs-lookup"><span data-stu-id="75d7c-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
