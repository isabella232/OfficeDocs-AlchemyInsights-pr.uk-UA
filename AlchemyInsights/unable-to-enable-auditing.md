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
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="e1382-102">Не вдається ввімкнути єдиний аудит</span><span class="sxs-lookup"><span data-stu-id="e1382-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="e1382-103">Під час спроби ввімкнути єдиний аудит для організації може з'явитися повідомлення про помилку, подібне до таких:</span><span class="sxs-lookup"><span data-stu-id="e1382-103">When you try to enable unified auditing for your organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="e1382-104">Щоб вирішити цю проблему, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="e1382-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="e1382-105">[Підключіться до Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="e1382-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="e1382-106">Запустіть наведений нижче командлет.</span><span class="sxs-lookup"><span data-stu-id="e1382-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="e1382-107">Зачекайте, доки не буде застосовано значення 60 хвилин для попереднього налаштування.</span><span class="sxs-lookup"><span data-stu-id="e1382-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="e1382-108">Виконайте таку команду в службі Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="e1382-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="e1382-109">Щоб отримати додаткові відомості, ознайомтеся з такими статтями:</span><span class="sxs-lookup"><span data-stu-id="e1382-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="e1382-110">Підключення до Exchange Online PowerShell за допомогою багатофакторної автентифікації</span><span class="sxs-lookup"><span data-stu-id="e1382-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="e1382-111">Увімкнення або вимкнення пошуку в журналі аудиту</span><span class="sxs-lookup"><span data-stu-id="e1382-111">Turn audit log search on or off</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
