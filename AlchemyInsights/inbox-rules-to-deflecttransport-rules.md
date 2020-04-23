---
title: 929 правила для вхідних повідомлень, щоб Деспутаправила транспортування
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "929"
- "1800021"
ms.assetid: 9733ef4e-db8d-4345-a072-c251480875a1
ms.openlocfilehash: 6b6e64c0332a579e8f6132b08f2f89b15eb4de27
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43724613"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a><span data-ttu-id="01fb8-102">Правила потоку пошти (також відомі як правила транспортування)</span><span class="sxs-lookup"><span data-stu-id="01fb8-102">Mail flow rules (also known as transport rules)</span></span>

- <span data-ttu-id="01fb8-103">Загальний огляд правил потоку пошти: [правила потоку пошти (правила транспортування) в Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span><span class="sxs-lookup"><span data-stu-id="01fb8-103">General overview of mail flow rules: [Mail flow rules (transport rules) in Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span></span>

- <span data-ttu-id="01fb8-104">Настроювання потоку пошти правила: [пошта потоків правила процедури в Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span><span class="sxs-lookup"><span data-stu-id="01fb8-104">Setup mail flow rules: [Mail flow rule procedures in Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span></span>

- <span data-ttu-id="01fb8-105">Створення, змінення та видалення правил потоку пошти: [керування правилами потоку пошти](https://technet.microsoft.com/library/jj657505.aspx)</span><span class="sxs-lookup"><span data-stu-id="01fb8-105">Create, modify, and delete mail flow rules: [Manage mail flow rules](https://technet.microsoft.com/library/jj657505.aspx)</span></span>

<span data-ttu-id="01fb8-106">Можна також керувати правилами потоку пошти в Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="01fb8-106">You can also manage mail flow rules in Exchange Online PowerShell.</span></span> <span data-ttu-id="01fb8-107">Більш детальну інформацію дивіться на « [Get-транспортроли](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) » (View), « [новий-транспортрил](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) » («створити»), « [видалення-транспортлу](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) » (Delete), « [Set-транспортроли](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) » (модифікують існуючі), [відключають-транспортви](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (відключаємо існуючі), і [дозволяють-транспортрять](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule)</span><span class="sxs-lookup"><span data-stu-id="01fb8-107">For more information, see [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (view), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (modify existing), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (disable existing), and [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (enable existing).</span></span>

<span data-ttu-id="01fb8-108">Додаткові правила потоку пошти командлети: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (список доступних дій), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (список доступних умов і винятків), [експорт-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (експорт правил), і [Імпорт-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (правила імпорту).</span><span class="sxs-lookup"><span data-stu-id="01fb8-108">Additional mail flow rule cmdlets: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (list available actions), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (list available conditions and exceptions), [Export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (export rules), and [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (import rules).</span></span>
