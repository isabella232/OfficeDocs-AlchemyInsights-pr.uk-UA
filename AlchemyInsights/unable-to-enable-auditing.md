---
title: 2419-для увімкнути аудит
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 3af01c03711eed646f0009afb5bea685bc358196
ms.sourcegitcommit: 87153fec6f6468b57893abf4aac073ba4068e67b
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/19/2019
ms.locfileid: "35065725"
---
# <a name="unable-to-enable-unified-auditing"></a>Не вдається увімкнути уніфікований аудит

Коли ви намагаєтеся ввімкнути уніфікованих аудиту поштових скриньок для організації Office 365, може з'явитися повідомлення про помилку, схоже нижче:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Щоб вирішити цю проблему, виконайте такі дії:

1. [Підключитися до обміну онлайн Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Запустіть наступну команду:

   ```
   Enable-OrganizationCustomization
   ```

3. Чекати на 60 хвилин для попередньої настройки вступили в силу.

4. Запустіть таку команду в Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Щоб отримати додаткові відомості перегляньте наступні статті:

- [Підключитися до Exchange Online PowerShell багатофакторну автентифікацію](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Вмикається Office 365 аудиту журнал пошуку](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
