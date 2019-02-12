---
title: Пересунути повідомлення електронної пошти до поштової скриньки архіву
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: a631af20e28a531a40f078e290239a372c38ab74
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29941735"
---
Проблеми архівування елементів поштової скриньки архіву. Переконайтеся, що ви виконали наведені нижче кроки:
  
1. Переконайтеся, що **архівувати поштової скриньки** ввімкнено. Якщо ні, то виконайте дії в [цій статті](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) , щоб увімкнути архівну поштову скриньку. 
    
2. Обмін центру адміністрування виберіть **Теги збереження** під **Управлінням дотримання**, створити **тег збереження** з дією **переміщення до архіву** до потрібного **Терміну збереження**.
    
3. Обмін центру адміністрування виберіть **Політики збереження**, створювати **Політику збереження** та додати ваш тег збереження **переміщення до архіву** до цієї політики. 
    
4. [Призначити політику збереження](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) до конкретного користувача поштової скриньки. Ту ж політику буде застосовано до **первинної** і поштової скриньки **архіву** . 
    
Поштову скриньку користувача тепер повинні мати політику архівування для переміщення елементів до поштової скриньки архіву. Можливо, буде необхідно для примусового Керовані папки помічник (МЗС) для запуску і застосувати нові параметри для поштової скриньки користувача. Запустіть таку команду під час [підключення до EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) , щоб запустити помічник із керованих папок для певної поштової скриньки: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Додаткові відомості про створення політику архівування, див. [Настроювання архіву і видалення політики поштових скриньок](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

