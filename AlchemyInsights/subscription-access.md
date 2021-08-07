---
title: Доступ до передплати
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
- "9003799"
- "6805"
ms.openlocfilehash: b138c05e87e70c18bb6528819a34f8a9501446d57dcf4dbac0734f70fbc3466b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999261"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Не вдається ввійти в Azure через проблеми з браузером (браузер "зависає", "зависає", "не завантажується" тощо).

На вас може впливати перебій. Перевірте, чи немає вихідних перебоїв: [Стан Azure Health.](https://status.azure.com/status/history/)

Вийдіть з усіх активних сеансів Azure. Запуск приватного або анонімного режиму браузера.

Якщо наведені вище дії не працюють, можна також спробувати оновити браузер, скористатись іншим браузером, видалити файли cookie кеша.

Докладні відомості: [Виправлення неполадок із входом](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Не вдається отримати доступ до передплат**

На [порталі Azure переконайтеся,](https://portal.azure.com/)що з облікового запису у верхньому правому куті вибрано правильний каталог Azure.

У Центрі [облікових записів Azure](https://account.windowsazure.com/Subscriptions)переконайтеся, що використовується обліковий запис адміністратора.

Докладні відомості: Виправлення [неполадок, пов'язаних із відсутності передплат](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Не вдається отримати доступ до журналу виставлення рахунків**

Адміністратор облікового запису повинен переконатися, що користувач, який має доступ до відомостей для виставлення рахунків, додається до azure Active Directory як гість: Додавання або видалення [нового користувача.](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support)

Потім користувачу потрібно призначити роль глобального адміністратора: [Призначити роль користувачам.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support)

Опублікувати це, користувач може отримати доступ до виставлення рахунків за допомогою політик RBAC: [надати доступ до виставлення рахунків.](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)

**Рекомендовані документи**

-   [Не вдається ввійти, щоб керувати передплатою Azure](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)