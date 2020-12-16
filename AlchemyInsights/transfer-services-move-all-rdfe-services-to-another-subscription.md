---
title: Перенесення служб – переміщення всіх служб RDFE до іншої передплатою
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
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692425"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Перенесення служб – переміщення всіх служб RDFE до іншої передплатою

**Переміщення ресурсів**

Блакитні ресурси можна переміщати в іншу абонентську або групу ресурсів в межах однієї передплатою, використовуючи Azure Portal, Azure PowerShell, Azure CLI або API REST для переміщення ресурсів.

Перш ніж переходити до ресурсів, див.:

- [Контрольний список перед переміщенням ресурсів](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Служби, які можна переміщати](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Перевірка переміщення](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Переміщення рекомендацій для служб](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Щоб перенести доступні ресурси до іншої групи ресурсів або передплатою, можна скористатися:

- [Портал «Лазурний»](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Блакитний PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Блакитний CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [API REST](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Навчальний посібник: [переміщення блакитного ресурсу до іншої групи ресурсів або передплатою](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Виправлення неполадок із диспетчером ресурсів Azure**

Зверніться до статей нижче, щоб дізнатися про деякі поширені помилки в Лазурне розгортання та отримувати інформацію, щоб їх вирішити. Якщо ви не можете знайти код помилки для вашої помилки розгортання, перегляньте статтю [знайти код помилки](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Виправлення помилок розгортання](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Виправлення неполадок із переміщенням лазурових ресурсів до нової групи ресурсів або передплатою](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Зверніть увагу, що якщо ви хочете оновити свою безкоштовну передплатну розсилку, наприклад перехід від безкоштовного до оплати, як-от-го, вам потрібно буде перетворити свою абонентську плату.

- Щоб оновити безкоштовну ознайомлювальну версію, ознайомтеся з [оновленням безкоштовного ознайомлювального або Microsoft Уявіть, що ви хочете сплатити за передплату](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).
- Щоб змінити обліковий запис "сплатити за вас", Дізнайтеся, [як перейти до іншої пропозиції](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).

**Щоб додати або пов'язати "Лазурний" для клієнта Azure Active Directory, зробіть ось що:**

1. Увійдіть у службу та виберіть передплату, яку потрібно використовувати на [сторінці "передплати" на порталі Azure Portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).
2. Виберіть **змінити каталог**.
3. Перегляньте всі попередження, які відображатимуться, а потім натисніть кнопку **змінити**.
4. Каталог буде змінений для передплатою, і ви отримаєте повідомлення про успішне.
5. Скористайтеся перемикачем *каталогів* , щоб перейти до нового каталогу. Це може тривати до 10 хвилин, щоб усі відображалися належним чином.

**Рекомендовані документи**

- [Передача права власності на Лазурне](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Переміщення ресурсів до нової групи ресурсів або передплатою](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Керування ресурсами за допомогою порталу "Лазурний"](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
