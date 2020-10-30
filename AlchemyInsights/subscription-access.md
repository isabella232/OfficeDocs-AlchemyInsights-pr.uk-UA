---
title: Доступ до передплатою
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
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807726"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Не вдається ввійти в Azure через проблеми з браузером (браузер зависає, продовжує обертатися, не завантажується і т. д.)

Можливо, під час відключення ви можете зіткнутися. Перевірте, чи є постійний процес відключення: « [блакитний стан здоров'я](https://status.azure.com/status/history/)».

Вийдіть із усіх активних сесій Лазур. Запустіть власний або режим анонімного перегляду веб-браузера.

Крім того, можна спробувати оновити браузер, використовувати інший браузер, видалити файли cookie кеша, якщо вище не працює.

Додаткові відомості: [усунення проблем із входом](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Не вдається отримати доступ до передплати**

Переконайтеся, [що в полі "обліковий](https://portal.azure.com/)запис" у верхньому правому куті вибрано потрібний каталог "Лазурний".

Переконайтеся, що для облікового запису, який використовується для адміністратора облікового запису, вибрано [пункт](https://account.windowsazure.com/Subscriptions)обліковий запис.

Додаткові відомості: [Виправлення неполадок із передплатою не знайдено](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Не вдається отримати доступ до журналу рахунків**

Адміністратор облікового запису повинен переконатися, що користувач, який має доступ до відомостей про виставлення рахунків, додається в "Блакитний Active Directory" як гостьовий користувач: [Додавання або видалення нового користувача](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

Користувач має надати роль глобального адміністратора: [призначити роль для користувачів](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Після цього користувач може надати доступ до рахунків за допомогою політики RBAC: [надати доступ до рахунків](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**Рекомендовані документи**

-   [Я не можу ввійти, щоб керувати передплатою на Лазурне](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)