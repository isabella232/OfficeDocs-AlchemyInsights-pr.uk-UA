---
title: Отримання списку корпоративних програм
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
- "9004342"
- "9837"
ms.openlocfilehash: 99e4f7e676610103355736ce847930c6c5d2d7532c4756ac4551a8d9b3020176
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54116749"
---
# <a name="get-a-list-of-enterprise-applications"></a>Отримання списку корпоративних програм

1. Список **корпоративних** програм (усі програми або відфільтровано за коротким ім'ям, ідентифікатором, ідентифікатором ідентифікатора ідентифікатора тощо) за допомогою команди PowerShell, див. в статті [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).
2. Список основних об'єктів служби (усіх об'єктів або відфільтрованих за ідентифікатором) за допомогою команди PowerShell див. в статті [Get-AzureADServicePrincipal (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal)
3. Якщо потрібно отримати список **налаштованих програм SAML,** наведені нижче сценарії PowerShell можуть допомогти вам:

    Кожна програма – це програма OAuth або SAML (як у галереї, так і в інших програмах), у разі реєстрації в AAD створиться два об'єкти. Один називається об'єктом Application, а інший – об'єктом Principal служби. Якщо ви скинете властивості основного об'єкта служби за допомогою PowerShell, виявите, що з кожною програмою пов'язано певну кількість тегів:

    - У програмах OAuth знадобиться тег **"WindowsAzureActiveDirectoryIntegratedApp"**
    - У галереї SAML Apps буде позначено тег **"WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1"**
    - У програмах без колекції SAML знадобиться тег **"WindowsAzureActiveDirectoryCustomSingleSignOnApplication"**

    Таким чином, ви можете використовувати ці теги та з'ясувати, яка програма це таке. Тег **"WindowsAzureActiveDirectoryIntegratedApp"** часто використовується для всіх типів програм. За допомогою наведеного нижче фрагмента можна перелічено всі програми SAML (як у колекції, так і у колекції).

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    Докладні відомості див. в ційи: Визначення програм із підтримкою [SAML в Azure AD.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)

4. **Пошук і список лише веб-програм:** скористайтеся наведеною нижче командою, щоб отримати всі програми Azure AD з типом програми "Web app/API"

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT
5. **Знайдіть і вказуйте** лише власні програми: виконайте таку команду, щоб отримати всі програми для настільного комп'ютера або мобільного пристрою.

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT
6. Експорт усіх зареєстрованих відомостей про програму Azure AD до **файлу CSV:** Наведена нижче команда експортує до CSV-файлу всі програми Azure AD з потрібними докладними інформацією.

    - Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |
    - Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8

7. **Потрібно експортувати список невизначених програм Azure –** контрольний звіт

    Azure AD може відображати журнали програм лише протягом 30 днів, якщо ви маєте ліцензію на Azure AD Premium.
    Дані можна зберегти двома способами протягом понад 30 днів. API-API [звітування Azure AD](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) можна використовувати, щоб отримувати дані програмно та зберігати в базі даних. Крім того, можна інтегрувати контрольні журнали в систему SIEM сторонніх постачальників.

    Список програм можна також завантажити для всіх програм і програм, які на власника перелічено в розділі Azure Active Directory>Реєстрації програм>Завантажити>Усі програми та програми, що на які належить.

    Список програм за допомогою MS Graph див. в статті Список програм [– Microsoft Graph версії 1.0](https://docs.microsoft.com/graph/api/application-list) і тип ресурсу програми – Microsoft Graph [1.0.](https://docs.microsoft.com/graph/api/resources/application)
