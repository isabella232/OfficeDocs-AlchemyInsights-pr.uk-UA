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
ms.openlocfilehash: e2fb22f872be0eefc3b4b78b18cd09baffa66cda
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742454"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Політики збереження в Центр адміністрування Exchange

 **Проблема:** Створений або оновлений політики збереження в Центр адміністрування Exchange не застосовуються до поштових скриньок або елементи не переміщуються до поштової скриньки архіву або видалено. 
  
 **Кореневі причини:**
  
- Можливо, **помічник із керованих папок** не обробляв поштову скриньку користувача. Помічник із керованих папок намагається обробити кожну поштову скриньку в організації, розміщеній у хмарі, кожні сім днів. Якщо змінити тег збереження або застосувати іншу політику збереження до поштової скриньки, можна зачекати, доки керовану папку допоможе обробити поштову скриньку, або запустити командлет Start-керовану помічника, щоб запустити помічник із керованих папок для обробки певної поштової скриньки. Запуск цього командлета корисний для тестування або виправлення неполадок параметрів політики збереження або тегів збереження. Для отримання додаткових відомостей відвідайте [запустіть Помічник із керованих папок](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Рішення:** Запустіть таку команду, щоб запустити помічник із керованих папок для певної поштової скриньки:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Це також може статися, якщо на поштову скриньку **увімкнуто** **Retentionhold** . Якщо поштову скриньку було розміщено на RetentionHold, політика збереження поштової скриньки не оброблятиметься протягом цього часу. Для отримання додаткових параметрів на RetentionHold параметр відображається: [утримання збереження поштової скриньки](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Рішення:**
    
  - Перевірте стан RetentionHold налаштування на конкретну поштову скриньку в [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Запустіть таку команду, щоб **Вимкнути** retentionhold на конкретну поштову скриньку:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Тепер знову запустіть Помічник із керованих папок:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Примітка:** Якщо поштова скринька менше 10 МБ, помічник із керованих папок не буде автоматично обробляти поштову скриньку.
 
Щоб отримати додаткові відомості про політики збереження в Центр адміністрування Exchange див.:
- [Теги збереження та політики збереження](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Застосування політики збереження до поштових скриньок](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Додавання або видалення тегів збереження](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Як визначити тип утримання, розміщеного на поштовій скриньці](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
