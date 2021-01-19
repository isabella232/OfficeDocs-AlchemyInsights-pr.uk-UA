---
title: Виправлення неполадок із запросками користувачів
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
ms.openlocfilehash: 0f2a10b918fee067b167ab58ac2544a89e0c8ea1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901594"
---
# <a name="troubleshoot-guest-user-issues"></a>Виправлення неполадок із запросками користувачів

1. Щоб отримати вказівки з керування Гостьовим доступом до програм, перегляньте статтю [керування Гостьовим доступом за допомогою оглядів із використанням лазуровий доступ](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews).
1. [Додавання користувачів-гостей до каталогу на порталі Azure](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal): у цьому QuickStart ви зможете додати нового користувача-гостя до свого каталогу Лазур за допомогою порталу "Лазурний", надіслати запрошення та дізнатися, як виглядатиме процес викупу запрошення гостей.
1. [Додавання гостя користувача за допомогою PowerShell](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell): у цьому QuickStart ви можете скористатися командою New-AzureADMSInvitation, щоб додати одного гостя до свого блакитного клієнта.
1. Щоб дізнатися, як призначити користувачів і групи, для корпоративних програм у лазурому Active Directory (Лазурне AD), на основі блакитного порталу або за допомогою PowerShell, перегляньте статтю [керування призначенням користувача для програми в "Блакитний" Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal). 
1. Співпраця в мережі Azure Active Directory (Azure AD) працює з більшістю програм, які інтегруються з Azure AD. У цій [статті](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)ми пройдемо вказівки з настроювання деяких популярних програм SaaS для використання в службі AZURE AD B2B.
1. Як організація, що використовує можливості співпраці в службі Azure Active Directory (Azure AD), щоб запрошувати користувачів-гостей із організацій-партнерів до свого Лазурого, тепер ви можете надати користувачам ці B2B доступ до локальних програм. Ці локальні програми можуть використовувати автентифікацію на основі SAML або інтегровану автентифікацію Windows (IWA) за допомогою делегації з обмеженнями Kerberos (KCD). Щоб отримати докладніші відомості, ознайомтеся з [можливостями надання B2B-користувачів в лазуровий доступ до локальних програм](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises).
1. Дізнайтеся, як [надати доступ до хмарних ресурсів локально керованих облікових записів, використовуючи співпрацю Azure AD B2B](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud).