---
title: Виправлення неполадок користувачів-гостей
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004358"
- "7822"
ms.openlocfilehash: 9e6030919721b4c0805a26ca45d365f31d88894e86ea08225f47576e7d152047
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939400"
---
# <a name="troubleshoot-guest-user-issues"></a>Виправлення неполадок користувачів-гостей

1. Докладні відомості про керування гостьовим доступом до програм див. в розділі Керування гостьовим доступом [за допомогою відгуків про доступ до Azure AD.](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews)
1. Додайте користувачів-гостей до каталогу на порталі [Azure.](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)На цьому короткому посібнику ви додасте нового користувача-гостя до каталогу Azure AD через портал Azure, надішліть запрошення та погляньте, як виглядає процес отримання запрошення гостя.
1. [Додавання користувача-гостя](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell)за допомогою PowerShell. У цьому короткому посібнику скористайтеся командою New-AzureADMSInvitation, щоб додати одного користувача-гостя до клієнта Azure.
1. Щоб дізнатися, як призначати користувачів і групи корпоративним програмам у службі Azure Active Directory (Azure AD) на порталі Azure або за допомогою PowerShell, див. статті Керування призначенням користувачів для програми в [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal). 
1. Azure Active Directory (Azure AD) для співпраці B2B працює з більшістю програм, інтеграних з Azure AD. У цій [статті](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)описано, як налаштувати деякі популярні saaS-програми для використання з Azure AD B2B.
1. Як організація, яка використовує можливості співпраці B2B в Azure Active Directory (Azure AD), щоб запрошувати користувачів-гостей із партнерських організацій до Azure AD, тепер ви можете надати цим користувачам B2B доступ до локальних програм. Ці локальні програми можуть використовувати автентифікацію на основі SAML або інтегровану автентифікацію Windows (IWA) з обмеженою делегацією Kerberos (KCD). Докладні відомості див. [в статтях Надання користувачам B2B в Azure AD доступ до локальних програм.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)
1. Дізнайтеся, як надати локально керованим партнерам доступ до хмарних ресурсів за допомогою [співпраці Azure AD B2B.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)