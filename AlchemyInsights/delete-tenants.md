---
title: Видалення клієнта
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564876"
---
# <a name="delete-tenant"></a>Видалення клієнта

Щоб видалити Azure AD, переконайтеся, що:
- Ви – Глобальний адміністратор у каталозі.
- Ви не ввійшли в обліковий запис, який містить каталог за замовчуванням, як-от contoso.onmicrosoft.com у підписаних облікових записів, як-от admin@contoso.onmicrosoft.com.
- Видаліть усі активні програми в каталозі перед видаленням. Щоб видалити активні програми, перейдіть до реєстрацій програм і видаліть вже наведені програми.
- Немає активних передплат для будь-яких служб Microsoft Online, таких як Microsoft Azure, Office 365 або Azure AD Premium, пов'язані з каталогом. Передача передплати або прискорення скасування активної передплати за допомогою служби Azure та виставлення рахунків. Дізнайтеся більше про те, як скасувати передплату Office 365 і Azure. Щоб отримати вказівки щодо зв'язування або додавання наявної передплатою до клієнта, зверніться до статті [зв'язати або додайте до свого клієнта Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).
- Немає активної ліцензії. Щоб видалити ліцензії, Дізнайтеся, [як видалити ліцензію](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- У каталозі немає інших активних користувачів, крім себе, як Глобальний адміністратор, коли ви намагаєтеся видалити Azure AD. Видаліть будь-які інші активні користувачі та всі залежності від настроюваного імені домену в клієнті також повинні бути видалені, наприклад користувачі, створені за допомогою admin@contoso.com.

Докладні відомості про те, як виконати наведені нижче дії.
- Видаліть "Azure Active Directory" або "Передплата", перегляньте статтю [DELETE Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Видаліть програми в каталозі, перегляньте статтю [видалення програм](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
