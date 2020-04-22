---
title: Переміщення повідомлень електронної пошти до поштової скриньки архіву
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: a5ad81e97df0ed5c337a622126173df94af80bb8
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713667"
---
# <a name="move-email-to-the-archive-mailbox"></a>Переміщення електронної пошти до поштової скриньки архіву

1. Переконайтеся, що **архівну поштову скриньку** ввімкнено. Якщо ні, виконайте дії, описані в [цій статті](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) , щоб увімкнути архівну поштову скриньку.

2. Щоб автоматично архівувати повідомлення до поштової скриньки архіву, тег збереження з дією « **перемістити в архів** » має бути встановлено для **автоматичного застосування до всієї поштової скриньки (за промовчанням)**. Використовуйте кроки тут, щоб створити тег: [Архів за замовчуванням](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Далі додайте тег **архіву** до політики збереження. У центрі адміністрування Exchange, виберіть політики **збереження** > додати **перемістити до архіву тег** політики > **зберегти**.

4. Тепер [призначте політику збереження](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) для конкретної поштової скриньки користувача. Цю саму політику буде застосовано до **основної** та **архівної** поштової скриньки.

Можливо, необхідно примусити помічника з керованих папок (МЗС) для запуску та застосування нових параметрів до поштової скриньки користувача. Виконайте таку команду під час [підключення до EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) , щоб запустити помічник із керованих папок для певної поштової скриньки:
  
Start-Управлінсья помічниці-тотожність<name of the mailbox>

Для отримання додаткових відомостей про настроювання політики архівування зверніться до [налаштування політики архівування та видалення для поштових скриньок](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  