---
title: Пошук відсутніх програм на blade реєстрації програми
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9654"
ms.openlocfilehash: 00b5821e2edad8b60ff60b1f85264d81c72277e4
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405225"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Пошук відсутніх програм на blade реєстрації програми

1. Не вдалося знайти програми на порталі реєстрації програм.

    Якщо програма зареєстрована в кількох клієнтах, вона не відображатиметься в розділі Реєстраційний блок програми. Однак ви можете знайти його в розділі "Корпоративні програми" після отримання доступу (після отримання згоди), а основне ім'я служби створено у вашому клієнта. Докладні відомості див. в статті & основних відомостей про служби [в Azure AD – платформа ідентичності Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
2. Не вдається переглянути програми в накладній реєстрації програм, навіть якщо ви адміністратор.

    Переконайтеся, що ви знаходитеся у відповідному каталозі на порталі Azure.
3. Моя програма не відображається в розділі Накладання корпоративних програм, але відображається під час виконання запиту до команди PowerShell.

    Іноді після видалення програми з порталу Azure вона не відображатися на порталі, але, можливо, її не видалено повністю. Докладні відомості:
    - Ви можете отримати список раніше видалених програм і дізнатися, чи програма відображається в списку за допомогою команди Powershell: **Get-AzureADDeletedApplication.** Докладні відомості див. [в статтях Get-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication)
    - Якщо потрібно повністю видалити програму, можна виконати такі дії в PowerShell: **Remove-AzureADApplication -ObjectId.** Докладні відомості див. [в статтях Видалення програми AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication)
    - Крім того, можна спробувати відновити видалену програму, використовуючи таку команду PowerShell: **Відновлення AzureADDeletedApplication -ObjectId.** Докладні відомості [див. в статтях Restore-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
4. Не вдається знайти список усіх попередньо інстальованих корпоративних програм у новому клієнта Azure.

    За замовчуванням в Azure AD попередньо інстальовано корпоративні програми. Її потрібно додати вручну з параметра "Нова програма", перейнявши її з колекції Azure AD або додавши програму, яка не є колекцією. Докладні відомості див. в короткому посібнику: додавання програми до клієнта [Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)
    Якщо ви глобальний адміністратор, ви можете легко отримувати доступ до програм за допомогою [запускача програм Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher)
5. Не вдалося знайти мої програми на порталі "Мої програми".

    Переконайтеся, що програми не приховано на сторінці "Колекція моїх програм". Докладні відомості див. [в статтях Колекції (попередній перегляд) на порталі "Мої програми" – Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections).
6. Відомості про запуск програм із порталу Мої програми див. в & використання програм на порталі Мої програми [– Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access).
7. Після інсталяції програма "Переміщення" в Office 365 не відображається на надлишку корпоративних програм.

    Програма "Office 365 Mover" – це багатофункціональна програма, яку не потрібно додавати до AAD за допомогою розділу "Програми колекції" в розділі "Реєстрація корпоративних програм". Щоб отримати доступ до програми "Переміщення" в Office 365, просто ввійдіть у програму й попросіть отримати згоду користувача на їх отримання. Коли користувач надасте згоду, ця програма автоматично додається до клієнта з ідентифікатором електронної пошти, у який ви ввійшли в систему.

    Після входу в програму запис цієї програми можна буде знайти в розділі blade програми Enterprise Applications в AAD. Вам потрібно знайти цю програму, ввівши повне ім'я, наприклад "Mover" (Office 365 Mover) або просто знайдіть "office", і програма має вказуватись у списку. Докладні відомості див. в розділі ["Перемістити програму" в Office 365:](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)її вже інстальовано, але вона не відображається в колекції корпоративних програм.
8. Короткий посібник. Перегляньте список програм, які використовують ваш компонент [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) для керування ідентичностями, щоб дізнатися, як переглядати програми, які вже називаються програмами, які вже настроєно на використання клієнта Azure AD як постачальника ідентичності.
9. [Виправлення поширених](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) проблем із додаванням або видаленням програми до Azure Active Directory допомагає зрозуміти поширені проблеми з переглядом програм в Azure Active Directory.
