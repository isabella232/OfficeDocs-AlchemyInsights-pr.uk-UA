---
title: Політики збереження Exchange центру адміністрування не працює
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 73e8db432afccb73b872ec7a3ce84c25f1ba7f25
ms.sourcegitcommit: ca06ef831226d629de3057a0df85e017b80f3356
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/08/2019
ms.locfileid: "29786791"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="3b104-102">Політики збереження Exchange центру адміністрування</span><span class="sxs-lookup"><span data-stu-id="3b104-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="3b104-103">**Питання:** Новостворених оновлений політиками Exchange центру адміністрування не докладаючи до поштових скриньок або є не переміщуються до поштової скриньки архіву та видаленні елементів.</span><span class="sxs-lookup"><span data-stu-id="3b104-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="3b104-104">**Корінних причин:**</span><span class="sxs-lookup"><span data-stu-id="3b104-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="3b104-p101">Це може бути тому, що з **Помічник керованих папок** не оброблено поштової скриньки користувача. Помічник із керованих папок намагається обробити кожну поштову скриньку у вашій хмарній організації один раз кожні сім днів. Якщо змінити тег збереження або застосовувати до поштової скриньки іншу політику збереження, ви можете чекати, поки на Керовані папки надання допомоги обробляє поштової скриньки, або ви можете запустити командлет Start-ManagedFolderAssistant, щоб запустити помічник із керованих папок для обробки певної Поштова скринька. Запуск цього командлета є корисним для перевірки або виправлення неполадок політики збереження або настройки тегів збереження. Для отримання додаткової інформації відвідайте [запустити помічник із керованих папок](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="3b104-p101">This may be because the **Managed Folder Assistant** has not processed the user's mailbox. The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days. If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox. Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings. For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="3b104-110">**Рішення:** Запустіть таку команду, щоб запустити помічник із керованих папок для певної поштової скриньки:</span><span class="sxs-lookup"><span data-stu-id="3b104-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span> 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="3b104-p102">Це може також бути виникнути, якщо **RetentionHold** був **включений** у поштовій скриньці. Якщо поштова скринька був зроблений на на RetentionHold, поштової скриньки, політика збереження не буде оброблено у цей час. Для більш інформація на RetentionHold настройку див: [Поштової скриньки збереження утримуйте](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="3b104-p102">This may also be occur if **RetentionHold** has been **enabled** on the mailbox. If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time. For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="3b104-114">**Рішення:**</span><span class="sxs-lookup"><span data-stu-id="3b104-114">**Solution:**</span></span>
    
  - <span data-ttu-id="3b104-115">Перевірити статус RetentionHold настройкам певної поштової скриньки у [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="3b104-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="3b104-116">Запустіть таку команду, щоб **Вимкнути** RetentionHold на певної поштової скриньки:</span><span class="sxs-lookup"><span data-stu-id="3b104-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span> 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="3b104-117">Тепер, повторно запустити помічник Керовані папки:</span><span class="sxs-lookup"><span data-stu-id="3b104-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="3b104-118">**Примітка:** Якщо поштової скриньки менше, ніж 10 МБ, помічник із керованих папок не буде автоматично оброблено поштової скриньки.</span><span class="sxs-lookup"><span data-stu-id="3b104-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span> 
  

