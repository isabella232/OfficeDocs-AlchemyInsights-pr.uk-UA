---
title: Переміщення повідомлень електронної пошти до поштової скриньки архіву
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
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799801"
---
# <a name="move-email-to-the-archive-mailbox"></a>Переміщення електронної пошти до поштової скриньки архіву

Якщо ви хочете, щоб ми могли виконати автоматичні перевірки для наведених нижче параметрів, натисніть кнопку назад, < – угорі цієї сторінки, а потім введіть адресу електронної пошти користувача, у якого виникли проблеми з переміщенням електронної пошти до поштової скриньки архіву.

1. Переконайтеся, що активовано **поштову скриньку архіву** . Якщо ні, виконайте кроки, описані в [цій статті](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) , щоб активувати поштову скриньку архіву.

2. Щоб автоматично архівувати повідомлення до архівної поштової скриньки, тег збереження з дією " **Перехід до архівування** " має бути настроєно **автоматично до всієї поштової скриньки (за замовчуванням)**. У цій статті описано, як створити тег: [Тег архіву за замовчуванням](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Потім додайте тег **архіву** до політики збереження. У центрі адміністрування Exchange виберіть **політики збереження** > додати **тег "Перехід до архіву** " до політики > " **зберегти**".

4. Тепер [призначте політику збереження](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) до поштової скриньки певного користувача. Цю саму політику буде застосовано до **основної** та **архівної** поштової скриньки.

Можливо, знадобиться примусово використовувати помічник із керованих папок (МЗС) для запуску та застосування нових настройок до поштової скриньки користувача. Щоб запустити помічник із керованих папок для певної поштової скриньки, виконайте таку команду, коли [підключаєтеся до EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) .
  
Початок-ManagedFolderAssistant-ідентичність <name of the mailbox>

Докладні відомості про настроювання політики архівування наведено в статті [Настроювання політики архівування та видалення для поштових скриньок](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  