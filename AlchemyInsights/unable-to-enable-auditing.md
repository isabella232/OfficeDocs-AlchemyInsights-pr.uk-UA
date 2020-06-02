---
title: 2419-не вдалося увімкнути-аудит
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 23ad07a6dd943d61d1bd45453089a771cfd51b58
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510449"
---
# <a name="unable-to-enable-unified-auditing"></a>Не вдалося ввімкнути уніфікований аудит

Під час спроби ввімкнення єдиного аудиту для організації, може з'явитися повідомлення про помилку, подібне до такого:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Щоб вирішити цю проблему, виконайте такі дії:

1. [Підключення до Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Виконайте такі команди:

   ```
   Enable-OrganizationCustomization
   ```

3. Зачекайте 60 хвилин для попереднього налаштування набрали сили.

4. Виконайте таку команду в Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Додаткові відомості можна отримати в таких статтях:

- [Підключення до Exchange Online PowerShell, використовуючи автентифікацію на кількох факторів](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Увімкнення та вимкнення пошуку журналу аудиту](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
