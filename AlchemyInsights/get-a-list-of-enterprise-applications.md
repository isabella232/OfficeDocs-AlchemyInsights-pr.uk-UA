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
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/26/2021
ms.locfileid: "51405508"
---
# <a name="get-a-list-of-enterprise-applications"></a><span data-ttu-id="00481-102">Отримання списку корпоративних програм</span><span class="sxs-lookup"><span data-stu-id="00481-102">Get a list of Enterprise Applications</span></span>

1. <span data-ttu-id="00481-103">Список **корпоративних** програм (усі програми або відфільтровано за коротким ім'ям, ідентифікатором, ідентифікатором ідентифікатора ідентифікатора тощо) за допомогою команди PowerShell, див. в статті [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span><span class="sxs-lookup"><span data-stu-id="00481-103">To **get a list of enterprise applications** (all applications or filtered by Display name, ID, Identifier URIs, etc.) through Powershell command, see [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span></span>
2. <span data-ttu-id="00481-104">Список основних об'єктів служби (усіх об'єктів або відфільтрованих за ідентифікатором) за допомогою команди PowerShell див. в статті [Get-AzureADServicePrincipal (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal)</span><span class="sxs-lookup"><span data-stu-id="00481-104">To get a list of service principal objects (all objects or filtered by ID) through Powershell command, see [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span></span>
3. <span data-ttu-id="00481-105">Якщо потрібно отримати список **налаштованих програм SAML,** наведені нижче сценарії PowerShell можуть допомогти вам:</span><span class="sxs-lookup"><span data-stu-id="00481-105">If you want to **get a list of SAML configured apps, following PowerShell scripts** may help you:</span></span>

    <span data-ttu-id="00481-106">Кожна програма – це програма OAuth або SAML (як у галереї, так і в інших програмах), у разі реєстрації в AAD створиться два об'єкти.</span><span class="sxs-lookup"><span data-stu-id="00481-106">Every Application be it an OAuth app or SAML app (both gallery and non-gallery apps) would have two objects created in AAD when their registration happens.</span></span> <span data-ttu-id="00481-107">Один називається об'єктом Application, а інший – об'єктом Principal служби.</span><span class="sxs-lookup"><span data-stu-id="00481-107">One is called the Application Object and the other is the Service Principal object.</span></span> <span data-ttu-id="00481-108">Якщо ви скинете властивості основного об'єкта служби за допомогою PowerShell, виявите, що з кожною програмою пов'язано певну кількість тегів:</span><span class="sxs-lookup"><span data-stu-id="00481-108">When you dump the properties of a Service Principal Object using PowerShell, you would find that every application has a certain number of Tags associated with it like:</span></span>

    - <span data-ttu-id="00481-109">У програмах OAuth знадобиться тег **"WindowsAzureActiveDirectoryIntegratedApp"**</span><span class="sxs-lookup"><span data-stu-id="00481-109">OAuth apps would have a tag called "**WindowsAzureActiveDirectoryIntegratedApp**"</span></span>
    - <span data-ttu-id="00481-110">У галереї SAML Apps буде позначено тег **"WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1"**</span><span class="sxs-lookup"><span data-stu-id="00481-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span></span>
    - <span data-ttu-id="00481-111">У програмах без колекції SAML знадобиться тег **"WindowsAzureActiveDirectoryCustomSingleSignOnApplication"**</span><span class="sxs-lookup"><span data-stu-id="00481-111">Non-Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span></span>

    <span data-ttu-id="00481-112">Таким чином, ви можете використовувати ці теги та з'ясувати, яка програма це таке.</span><span class="sxs-lookup"><span data-stu-id="00481-112">Hence, you can use these tags and find out what kind of app it is.</span></span> <span data-ttu-id="00481-113">Тег **"WindowsAzureActiveDirectoryIntegratedApp"** часто використовується для всіх типів програм.</span><span class="sxs-lookup"><span data-stu-id="00481-113">The tag "**WindowsAzureActiveDirectoryIntegratedApp**" is common to all types of apps.</span></span> <span data-ttu-id="00481-114">За допомогою наведеного нижче фрагмента можна перелічено всі програми SAML (як у колекції, так і у колекції).</span><span class="sxs-lookup"><span data-stu-id="00481-114">You can use following snippet to list all the SAML apps (both gallery and non-gallery):</span></span>

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    <span data-ttu-id="00481-115">Докладні відомості див. в ційи: Визначення програм із підтримкою [SAML в Azure AD.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)</span><span class="sxs-lookup"><span data-stu-id="00481-115">For more information, see [Identify SAML-enabled apps in Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span></span>

4. <span data-ttu-id="00481-116">**Пошук і список лише веб-програм:** скористайтеся наведеною нижче командою, щоб отримати всі програми Azure AD з типом програми "Web app/API"</span><span class="sxs-lookup"><span data-stu-id="00481-116">**Find and list only Web applications**: Use the below command to get all Azure AD applications with the application type "Web app/API"</span></span>

    <span data-ttu-id="00481-117">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT</span><span class="sxs-lookup"><span data-stu-id="00481-117">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -ne $true } | FT</span></span>
5. <span data-ttu-id="00481-118">**Знайдіть і вказуйте** лише власні програми: виконайте таку команду, щоб отримати всі програми для настільного комп'ютера або мобільного пристрою.</span><span class="sxs-lookup"><span data-stu-id="00481-118">**Find and list Native applications alone**: Run the following command to get all the native client (desktop/mobile device) applications.</span></span>

    <span data-ttu-id="00481-119">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT</span><span class="sxs-lookup"><span data-stu-id="00481-119">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -eq $true } | FT</span></span>
6. <span data-ttu-id="00481-120">Експорт усіх зареєстрованих відомостей про програму Azure AD до **файлу CSV:** Наведена нижче команда експортує до CSV-файлу всі програми Azure AD з потрібними докладними інформацією.</span><span class="sxs-lookup"><span data-stu-id="00481-120">**Export All Registered Azure AD Application Details to CSV**: The below command exports all the Azure AD apps with required details to csv file:</span></span>

    - <span data-ttu-id="00481-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span><span class="sxs-lookup"><span data-stu-id="00481-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span></span>
    - <span data-ttu-id="00481-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span><span class="sxs-lookup"><span data-stu-id="00481-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span></span>

7. <span data-ttu-id="00481-123">**Потрібно експортувати список невизначених програм Azure –** контрольний звіт</span><span class="sxs-lookup"><span data-stu-id="00481-123">**Need to export a list of unused Azure apps** – Audit report</span></span>

    <span data-ttu-id="00481-124">Azure AD може відображати журнали програм лише протягом 30 днів, якщо ви маєте ліцензію Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="00481-124">Azure AD can show application logs for only up to 30 days provided you have Azure AD Premium license.</span></span>
    <span data-ttu-id="00481-125">Дані можна зберегти двома способами протягом понад 30 днів.</span><span class="sxs-lookup"><span data-stu-id="00481-125">You have two options to retain the data for longer than 30 days.</span></span> <span data-ttu-id="00481-126">API-API [звітування Azure AD](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) можна використовувати, щоб отримувати дані програмно та зберігати в базі даних.</span><span class="sxs-lookup"><span data-stu-id="00481-126">You can use the [Azure AD Reporting APIs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) to retrieve the data programmatically and store it in a database.</span></span> <span data-ttu-id="00481-127">Крім того, можна інтегрувати контрольні журнали в систему SIEM сторонніх постачальників.</span><span class="sxs-lookup"><span data-stu-id="00481-127">Alternatively, you can integrate audit logs into a third party SIEM system.</span></span>

    <span data-ttu-id="00481-128">Список програм можна також завантажити для всіх програм і програм, які на власника перелічено в розділі Azure Active Directory>Реєстрації програм>Завантажити>Усі програми та програми, що на які належить.</span><span class="sxs-lookup"><span data-stu-id="00481-128">You can also download the app list for all applications and owned applications under Azure Active directory>App Registrations>Download>All applications/Owned applications.</span></span>

    <span data-ttu-id="00481-129">Список програм за допомогою MS Graph див. в статті Список програм [– Microsoft Graph 1.0](https://docs.microsoft.com/graph/api/application-list) і тип ресурсу програми [– Microsoft Graph 1.0.](https://docs.microsoft.com/graph/api/resources/application)</span><span class="sxs-lookup"><span data-stu-id="00481-129">To get a list of applications through MS Graph, see [List applications - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) and [application resource type - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span></span>
