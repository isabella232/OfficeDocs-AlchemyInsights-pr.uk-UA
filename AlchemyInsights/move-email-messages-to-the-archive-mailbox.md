---
title: Переміщення повідомлень електронної пошти до архівних поштових скриньок
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
ms.openlocfilehash: 7e72766f441e210a81fcfd6c07b1801f6c0474afb02a70edf2ad8dbb571f3d2a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974978"
---
# <a name="move-email-to-the-archive-mailbox"></a>Переміщення електронної пошти до архівних поштових скриньок

Якщо ви хочете, щоб ми виконували автоматичні перевірки наведених нижче параметрів, натисніть кнопку "Назад" < – у верхній частині цієї сторінки, а потім введіть адресу електронної пошти користувача, у якого виникли проблеми з переміщенням електронної пошти до архівної поштової скриньки.

1. Переконайтеся, що **архівну поштову** скриньку активовано. Якщо ні, виконайте кроки, [описані в цій статті,](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) щоб увімкнути архівування поштової скриньки.

2. Щоб автоматично архівувати повідомлення до архівної поштової  скриньки, позначку збереження з дією "Перемістити до архіву" потрібно налаштувати на автоматичне застосування до всієї позначки **поштової скриньки (за замовчуванням).** Щоб створити позначку, виконайте наведені нижче [дії.](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)

3. Потім додайте **позначку Архів** до політики збереження. У Центрі Exchange адміністрування виберіть  Політики збереження> додайте **тег "Перемістити** до архіву" до політики, > **Зберегти.**

4. Тепер [призначте політику збереження](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) поштовій скриньці певного користувача. Ту саму політику буде застосовано як до **основної,** так і до **архівної поштової** скриньки.

Можливо, потрібно буде змусити помічник із керованих папок (MFA) запускати й застосовувати нові параметри до поштової скриньки користувача. Щоб запустити помічник із керованих папок для певної поштової скриньки, підключіться до [EXO PowerShell,](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) виконайте таку команду:
  
Start-ManagedFolderAssistant -Identity <name of the mailbox>

Докладні відомості про налаштування політики архівування див. в сторінці Налаштування політики архівування та видалення для [поштових скриньок.](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)
  