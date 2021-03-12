---
title: Створити користувача
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
ms.openlocfilehash: 742ff857141d08031302fdcff7e49b3eef90e0f7
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747031"
---
# <a name="create-user"></a>Створити користувача

**ОГОЛОШЕННЯ**

- [Припинення роботи входу в WebView від Google починаючи з 4 січня 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) . Перевірте, чи можуть ваші програми залежати від Google, дотримуючись [вказівок](https://go.microsoft.com/fwlink/?linkid=2157323) з перевірки сумісності.
- Переконайтеся, що ви використовуєте веб-подання системи або системний браузер під час входу користувачів зі службою споживчого облікового запису Google. Щоб отримати докладніші відомості, перегляньте [проблеми з входом у програму лише за допомогою браузера Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).

**Не вдається створити нового користувача в папці "мій Лазурний РЕКЛАМНИЙ"**

1. Переконайтеся, що ви надали дозвіл на створення нового стандартного користувача. Створити новий стандартний користувач може лише Глобальний адміністратор або роль адміністратора користувача в Лазурому Active Directory (AD). Якщо ви не в одній із цих ролей, попросіть адміністратора додати вас до однієї з цих ролей або створити новий обліковий запис користувача.
1. Переконайтеся, що ім'я користувача перебуває в домені, який перевіряється в Лазурному ОГОЛОШЕННІ. Якщо у вас немає жодного перевіреного настроюваного імені домену в Лазурному ОГОЛОШЕННІ, ви можете скористатися вашим початковим доменом Azure AD, що завершується *. onmicrosoft.com.
1. Переконайтеся, що ім'я користувача перебуває в домені, який не є федеративним для Azure AD від локального РЕКЛАМНОГО користувача. Користувачі не можуть додавати до хмари з іменами доменів, які є федеративними в локальних.
1. Переконайтеся, що інший користувач або контакт уже має ім'я користувача, яке потрібно призначити новому користувачу. Імена користувачів мають бути унікальними в межах Лазурого AD.
1. Переглядайте [блакитні ролі та адміністратори](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) в лазурому оголошенні.
1. Перегляньте [імена доменів](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) для свого AZURE AD.
1. Перегляньте [журнали аудиту](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) , щоб переглянути докладні відомості про нещодавно створений або видалений користувач, який виконав дію та коли.
1. Щоб отримати докладні відомості про додавання нових користувачів, перегляньте статтю [використання порталу "Лазурний" для створення нового користувача в Лазур](/azure/active-directory/active-directory-users-create-azure-portal).
1. [Блакитні ролі адміністрування Azure](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles): дозволи для ролі адміністратора в "Блакитний" Active Directory
1. [Для створення нового користувача також можна використовувати Azure AD PowerShell](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).
