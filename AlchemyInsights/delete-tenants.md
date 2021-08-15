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
ms.openlocfilehash: 7377f77b7295e8134673c9a46fa7606842d4df949f535878d13986c6d39d0b5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53993914"
---
# <a name="delete-tenant"></a>Видалення клієнта

Щоб видалити Azure AD, переконайтеся, що:
- Ви – глобальний адміністратор у каталозі.
- Ви НЕ ввійшли за допомогою облікового запису, який має стандартний каталог, наприклад contoso.onmicrosoft.com обліковий запис для входу, наприклад admin@contoso.onmicrosoft.com.
- Перш ніж видаляти всі активні програми з каталогу, видаліть їх. Щоб видалити активні програми, перейдіть до реєстрацій програм і видаліть наявні програми.
- Активні передплати на будь-які служби Microsoft Online Services, як-от Microsoft Azure, Office 365 або Azure AD, пов'Premium у каталозі. Перенесіть передплати або шахрайське скасування активних передплат через підтримку Azure та виставлення рахунків. Докладні відомості див. в статті Office 365 та Передплати Azure. Докладні відомості про те, як пов'язати або додати наявну передплату до клієнта, див. в статтях Зв'язування або додавання передплати Azure до [клієнта Azure AD.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)
- Немає активної ліцензії. Відомості про вилучення ліцензій див. [в статті Вилучення передплати на видалення ліцензії.](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription)
- Під час спроби видалити Azure AD інші активні користувачі не беруться до себе як глобальний адміністратор. Видаліть будь-яких інших активних користувачів, і будь-які залежності від імені настроюваного домену в цьому компоненті також знадобиться видалити, наприклад користувачів, створених за допомогою admin@contoso.com.

Докладні інструкції див. в цих статтях:
- Видаліть "Azure Active Directory" або "передплату", див. [Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto)
- Відомості про видалення програм із каталогу див. в [цій сторінці.](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app) 
