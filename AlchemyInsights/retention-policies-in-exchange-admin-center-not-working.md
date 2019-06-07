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
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 56c2bea5e205358d0ef29fa937e36a88ffc46a1e
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/07/2019
ms.locfileid: "34761603"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Політики збереження Exchange центру адміністрування

 **Питання:** Новостворених оновлений політиками Exchange центру адміністрування не докладаючи до поштових скриньок або є не переміщуються до поштової скриньки архіву та видаленні елементів. 
  
 **Корінних причин:**
  
- Це може бути тому, що з **Помічник керованих папок** не оброблено поштової скриньки користувача. Помічник із керованих папок намагається обробити кожну поштову скриньку у вашій хмарній організації один раз кожні сім днів. Якщо змінити тег збереження або застосовувати до поштової скриньки іншу політику збереження, ви можете чекати, поки на Керовані папки надання допомоги обробляє поштової скриньки, або ви можете запустити командлет Start-ManagedFolderAssistant, щоб запустити помічник із керованих папок для обробки певної Поштова скринька. Запуск цього командлета є корисним для перевірки або виправлення неполадок політики збереження або настройки тегів збереження. Для отримання додаткової інформації відвідайте [запустити помічник із керованих папок](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Рішення:** Запустіть таку команду, щоб запустити помічник із керованих папок для певної поштової скриньки: 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Це може також бути виникнути, якщо **RetentionHold** був **включений** у поштовій скриньці. Якщо поштова скринька був зроблений на на RetentionHold, поштової скриньки, політика збереження не буде оброблено у цей час. Для більш інформація на RetentionHold настройку див: [Поштової скриньки збереження утримуйте](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Рішення:**
    
  - Перевірити статус RetentionHold настройкам певної поштової скриньки у [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Запустіть таку команду, щоб **Вимкнути** RetentionHold на певної поштової скриньки: 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Тепер, повторно запустити помічник Керовані папки:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Примітка:** Якщо поштової скриньки менше, ніж 10 МБ, помічник із керованих папок не буде автоматично оброблено поштової скриньки. 
  

