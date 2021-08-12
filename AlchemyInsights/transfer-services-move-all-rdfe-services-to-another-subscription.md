---
title: Перенесення служб. Перенесення всіх служб RDFE до іншої передплати
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004116"
- "7196"
ms.openlocfilehash: 89217922b8b51f2548f9fff53bf80364c0e897b1d9b34bfb7016f0b0f197cf17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940114"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Перенесення служб. Перенесення всіх служб RDFE до іншої передплати

**Переміщення ресурсів**

Ресурси Azure можна перенести до іншої передплати або групи ресурсів Azure за однією передплатою на портал Azure, Azure PowerShell, Azure CLI або REST API, щоб перемістити ресурси.

Перш ніж переміщати ресурси, див.:

- [Контрольний список перед переміщенням ресурсів](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Служби, які можна переміщати](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Перевірка переміщення](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Переміщення довідок для служб](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Щоб перемістити наявні ресурси до іншої групи ресурсів або передплати, можна використати:

- [Портал Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Навчальна [вправа: переміщення ресурсів Azure до іншої групи ресурсів або передплати](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Усунення несправностей у Диспетчері ресурсів Azure**

Відомості про деякі поширені помилки розгортання Azure та їх виправлення див. в наведених нижче статтях. Якщо не вдається знайти код помилки розгортання, див. знайдіть [код помилки](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Виправлення помилок розгортання](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Усунення несправностей переміщення ресурсів Azure до нової групи ресурсів або передплати](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Зверніть увагу: щоб оновити передплату на Azure, наприклад перейти з безкоштовної оплати в будь-який час, знадобиться перетворити передплату.

- Відомості про те, як оновити безкоштовну ознайомлювальну версію, див. в статті Оновлення безкоштовної ознайомлювальної версії або передплати на Microsoft Imagine Azure до версії [Pay-As-You-Go.](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)
- Щоб змінити обліковий запис, що почнеться, див. номери передплати на [Azure Pay-As-You-Go на іншу пропозицію.](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)

**Щоб додати або пов'язати передплату Azure з Azure Active Directory клієнта:**

1. Увійдіть і виберіть потрібну передплату на сторінці [Передплати на порталі Azure](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).
2. Виберіть **Змінити каталог**.
3. Перегляньте всі попередження, які з'являються, а потім натисніть **кнопку Змінити**.
4. Каталог змінюється для передплати, і ви отримаєте повідомлення про успіх.
5. Скористайтеся *перемикачем* каталогу, щоб перейти до нового каталогу. Щоб усе могло відбуватись належним чином, може знадатися до 10 хвилин.

**Рекомендовані документи**

- [Передавання права власності на передплату Azure](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Переміщення ресурсів до нової групи ресурсів або передплати](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Керування ресурсами за допомогою порталу Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
