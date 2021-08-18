---
title: Створення користувача
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: a144b172787563b1aa57bdec790df1805a13f078
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323307"
---
# <a name="create-user"></a>Створення користувача

**ОГОЛОШЕННЯ:**

- [Вилучення підтримки входу в WebView від Google із 4 січня 2021 р.](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) Перевірте, чи можуть на ваші програми вплинути наведені в [Google](https://go.microsoft.com/fwlink/?linkid=2157323) указівки щодо сумісності тестування.
- Увійдіть у систему за допомогою облікових записів Google споживачів і переконайтеся, що ви використовуєте системний веб-браузер або системний браузер. Докладні відомості див. в статтях Проблеми з входом лише в програми [за допомогою браузера Chrome.](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)

**Не вдається створити нового користувача в каталозі Azure AD**

1. Переконайтеся, що ви маєте право створювати нового стандартного користувача. Новий стандартний користувач може створити лише роль глобального Azure Active Directory адміністратора в Azure Active Directory (AD). Якщо ви не на одній із цих ролей, попросіть адміністратора додати вас до однієї з цих ролей або створити новий обліковий запис користувача для вас.
1. Переконайтеся, що ім'я користувача перевірено в Azure AD. Якщо в Azure AD немає перевірених імен настроюваних доменів, можна використовувати початковий домен Azure AD, який закінчується на *.onmicrosoft.com.
1. Переконайтеся, що ім'я користувача в домені, не ітерованому до Azure AD, з локальної служби AD. Користувачів не можна додавати до хмари з іменами доменів, іфедеративними з локальних доменів.
1. Переконайтеся, що жодний інший користувач або контакт не має імені користувача, яке потрібно призначити новому користувачу. Імена користувачів мають бути унікальні в Azure AD.
1. Див. [номери ролей і адміністраторів Azure AD](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) для Azure AD.
1. Перегляньте [імена доменів](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) для azure AD.
1. Перегляньте [контрольні журнали,](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) щоб переглянути докладніші відомості про нещодавно створеного або видаленого користувача (наприклад, тих, хто виконав дію) і час.
1. Докладні відомості про додавання нових користувачів див. в цій [статтях.](https://docs.microsoft.com/azure/active-directory/active-directory-users-create-azure-portal)
1. [Права адміністратора Azure AD: дозволи](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles)адміністратора в Azure Active Directory
1. Ви також можете [створити нового користувача за допомогою Azure AD PowerShell.](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)
