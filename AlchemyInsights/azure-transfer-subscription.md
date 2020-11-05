---
title: Передача права власності на Azure
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922174"
---
# <a name="transfer-azure-billing-ownership"></a>Передача права власності на Azure

Увійдіть на портал " [Лазурний](https://portal.azure.com/) " як адміністратор облікового запису для виставлення рахунка, який має передплатою, яку потрібно перенести. Якщо ви не впевнені, що ви маєте права адміністратора, або якщо вам потрібно визначити, хто є, перегляньте статтю [визначення адміністратора виставлення рахунків](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

- Пошук у службі **керування витратами + виставлення рахунків**.
- Виберіть пункт **передплати** з області ліворуч. Залежно від Access може знадобитися вибрати область виставлення рахунків, а потім **передплачений** або **блакитні передплати**.
- Виберіть пункт **передати право власності на виставлення рахунків** для передплатою, яку потрібно перенести.
- Введіть адресу електронної пошти користувача, який є адміністратором виставлення рахунків, який стане новим власником для передплатою, а потім натисніть кнопку **Надіслати запит на перенесення**
- Користувач отримує повідомлення електронної пошти з інструкціями, щоб переглянути ваш запит на перенесення. Щоб затвердити запит на перенесення, користувач вибирає посилання в електронному листі та відповідає інструкціям.

**Примітка**. Якщо ви переносите право власності на ваш обліковий запис для облікового запису користувача в іншому клієнті AZURE AD, усі завдання, які [базуються на рольовій службі керування доступом (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)для керування ресурсами в передплаті, остаточно видалено. Лише новий власник матиме доступ до керування ресурсами в передплаті. Докладні відомості наведено в статті [передавання передплатою користувачу в іншому клієнті Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Рекомендовані документи**

- [Передача права власності на «Лазурний» на інший обліковий запис](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Про передачу права власності на "Лазурний"](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Передача Visual Studio, Партнерська мережа Microsoft (MPN) і оплата під час переходу до dev/Test передплати](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Запитання й відповіді про права власності](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Усунення проблем із відповідним Передаваннями](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
