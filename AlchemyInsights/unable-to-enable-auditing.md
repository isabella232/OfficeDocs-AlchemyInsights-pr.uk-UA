---
title: 2419-unable-to-enable-auditing
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
ms.openlocfilehash: 0566a8d002b1bd9e38f3184824193394e49d56494d347338f96cfcdfdb758f4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007811"
---
# <a name="unable-to-enable-unified-auditing"></a>Не вдається ввімкнути уніфікований аудит

Коли ви намагаєтеся ввімкнути уніфікований аудит для організації, може з'явитися приблизно така помилка:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Щоб вирішити цю проблему, виконайте такі дії:

1. [Підключення, щоб Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)

2. Запустіть такий командлет:

   ```
   Enable-OrganizationCustomization
   ```

3. Зачекайте 60 хвилин, доки попередній параметр набере сили.

4. Виконайте в оболонці PowerShell Exchange Online таку команду:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Докладні відомості див. в таких статтях:

- [Підключення використовувати багатофакторна Exchange Online PowerShell за допомогою багатофакторна автентифікація](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Увімкнення або вимкнення пошуку в контрольних журналах](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
