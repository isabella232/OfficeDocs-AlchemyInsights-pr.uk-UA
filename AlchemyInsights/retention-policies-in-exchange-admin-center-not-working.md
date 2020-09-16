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
# <a name="retention-policies-in-exchange-admin-center"></a>Політики збереження в центрі адміністрування Exchange

Якщо ви хочете, щоб ми могли виконати автоматичні перевірки для наведених нижче параметрів, натисніть кнопку назад, < – угорі цієї сторінки, а потім введіть адресу електронної пошти користувача, який має проблеми з політиками збереження.

 **Проблема:** Щойно створені або оновлені політики збереження в центрі адміністрування Exchange не застосовуються до поштових скриньок або елементи, не переміщуються до архівної поштової скриньки або видаляються. 
  
 **Причини кореневої:**
  
- Можливо, це пояснюється тим, що **помічник керованої папки** не обробляється поштовою скринькою користувача. Помічник із керованих папок намагається виконати обробку кожної поштової скриньки в організації, що базується на хмарі, кожні сім днів. Якщо змінити тег збереження або застосувати іншу політику збереження до поштової скриньки, можна зачекати, доки керована папка допоможе обробити поштову скриньку або запустити командлет Start-ManagedFolderAssistant, щоб запустити помічник із керованих папок для обробки певної поштової скриньки. Запуск цього командлета стане в нагоді для тестування та виправлення неполадок політики збереження або параметрів тега збереження. Щоб отримати докладніші відомості, перейдіть на вкладку [Запуск помічника з керованих папок](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Рішення:** Щоб запустити помічник із керованих папок для певної поштової скриньки, виконайте таку команду:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Це також може виникати, якщо в поштовій скриньці **ввімкнуто функцію** **Reensionhold** . Якщо поштова скринька була розміщена на веб-сторінці, у цьому часі політику збереження в поштовій скриньці не буде оброблено. Для отримання додаткових відомостей про настроювання в розділі Reensionhold: [утримання збереження поштової скриньки](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Рішення**
    
  - Перевірте стан параметра "повторна перевірка" на певній поштовій скриньці в [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Виконайте таку команду, щоб **вимкнути функцію** reensionhold для певної поштової скриньки:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Тепер повторно запустіть Помічник із керованих папок:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Примітка.** Якщо поштова скринька менше 10 МБ, помічник із керованих папок автоматично обробляє поштову скриньку.
 
Докладні відомості про політики збереження в центрі адміністрування Exchange наведено в статті:
- [Позначки збереження та політики збереження](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Використання політики збереження в поштових скриньках](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Додавання та видалення тегів збереження](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Визначення типу утримання, розміщеного в поштовій скриньці](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
