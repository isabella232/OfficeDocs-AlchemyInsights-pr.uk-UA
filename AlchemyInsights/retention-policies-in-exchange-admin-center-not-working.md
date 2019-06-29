---
title: Політики збереження Exchange центру адміністрування не працює
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 9f4a175239bc20aaf489615da63ef35002030a70
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/28/2019
ms.locfileid: "35369686"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="cdebc-102">Політики збереження Exchange центру адміністрування</span><span class="sxs-lookup"><span data-stu-id="cdebc-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="cdebc-103">**Питання:** Новостворених оновлений політиками Exchange центру адміністрування не докладаючи до поштових скриньок або є не переміщуються до поштової скриньки архіву та видаленні елементів.</span><span class="sxs-lookup"><span data-stu-id="cdebc-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="cdebc-104">**Корінних причин:**</span><span class="sxs-lookup"><span data-stu-id="cdebc-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="cdebc-105">Це може бути тому, що з **Помічник керованих папок** не оброблено поштової скриньки користувача.</span><span class="sxs-lookup"><span data-stu-id="cdebc-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="cdebc-106">Помічник із керованих папок намагається обробити кожну поштову скриньку у вашій хмарній організації один раз кожні сім днів.</span><span class="sxs-lookup"><span data-stu-id="cdebc-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="cdebc-107">Якщо змінити тег збереження або застосовувати до поштової скриньки іншу політику збереження, ви можете чекати, поки на Керовані папки надання допомоги обробляє поштової скриньки, або ви можете запустити командлет Start-ManagedFolderAssistant, щоб запустити помічник із керованих папок для обробки певної Поштова скринька.</span><span class="sxs-lookup"><span data-stu-id="cdebc-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="cdebc-108">Запуск цього командлета є корисним для перевірки або виправлення неполадок політики збереження або настройки тегів збереження.</span><span class="sxs-lookup"><span data-stu-id="cdebc-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="cdebc-109">Для отримання додаткової інформації відвідайте [запустити помічник із керованих папок](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="cdebc-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="cdebc-110">**Рішення:** Запустіть таку команду, щоб запустити помічник із керованих папок для певної поштової скриньки:</span><span class="sxs-lookup"><span data-stu-id="cdebc-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="cdebc-111">Це може також бути виникнути, якщо **RetentionHold** був **включений** у поштовій скриньці.</span><span class="sxs-lookup"><span data-stu-id="cdebc-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="cdebc-112">Якщо поштова скринька був зроблений на на RetentionHold, поштової скриньки, політика збереження не буде оброблено у цей час.</span><span class="sxs-lookup"><span data-stu-id="cdebc-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="cdebc-113">Для більш інформація на RetentionHold настройку див: [Поштової скриньки збереження утримуйте](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="cdebc-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="cdebc-114">**Рішення:**</span><span class="sxs-lookup"><span data-stu-id="cdebc-114">**Solution:**</span></span>
    
  - <span data-ttu-id="cdebc-115">Перевірити статус RetentionHold настройкам певної поштової скриньки у [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="cdebc-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="cdebc-116">Запустіть таку команду, щоб **Вимкнути** RetentionHold на певної поштової скриньки:</span><span class="sxs-lookup"><span data-stu-id="cdebc-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="cdebc-117">Тепер, повторно запустити помічник Керовані папки:</span><span class="sxs-lookup"><span data-stu-id="cdebc-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="cdebc-118">**Примітка:** Якщо поштової скриньки менше, ніж 10 МБ, помічник із керованих папок не буде автоматично оброблено поштової скриньки.</span><span class="sxs-lookup"><span data-stu-id="cdebc-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
  