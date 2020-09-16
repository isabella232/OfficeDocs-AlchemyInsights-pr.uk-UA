---
title: 2419 – не вдалося ввімкнути функцію аудиту
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 81fd8e33feb2f2b10b04cc7cdc746a8603aa366b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767620"
---
# <a name="unable-to-enable-unified-auditing"></a>Не вдається ввімкнути єдиний аудит

Під час спроби ввімкнути єдиний аудит для організації може з'явитися повідомлення про помилку, подібне до таких:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Щоб вирішити цю проблему, виконайте наведені нижче дії.

1. [Підключіться до Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Запустіть наведений нижче командлет.

   ```
   Enable-OrganizationCustomization
   ```

3. Зачекайте, доки не буде застосовано значення 60 хвилин для попереднього налаштування.

4. Виконайте таку команду в службі Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Щоб отримати додаткові відомості, ознайомтеся з такими статтями:

- [Підключення до Exchange Online PowerShell за допомогою багатофакторної автентифікації](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Увімкнення або вимкнення пошуку в журналі аудиту](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
