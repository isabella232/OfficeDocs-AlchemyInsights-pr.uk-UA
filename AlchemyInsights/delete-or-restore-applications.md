---
title: Видалення або відновлення програм
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
- "9004335"
- "7737"
ms.openlocfilehash: 0c7be98650ca87f36b66f0bb38fb665fc81525b7f3410da14b99fb67468c1e73
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102592"
---
# <a name="delete-or-restore-applications"></a>Видалення або відновлення програм

**Щоб видалити програму з клієнта Azure AD:**

1. На **порталі Azure AD виберіть** **корпоративні програми**. Потім знайдіть і виберіть програму, яку потрібно видалити.
2. У розділі **Керування** в області ліворуч виберіть **Властивості**.
3. Виберіть **Видалити**, а потім **–** Так, щоб підтвердити видалення програми з клієнта Azure AD.

Докладні відомості про те, як видалити програму, див. в статті Короткий посібник. Видалення програми з клієнта [Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)

У PowerShell командлет [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) вилучає конфігурації проксі-сервера програм із певної програми в Azure Active Directory і може повністю видалити програму, якщо зазначено.

Видалену **програму можна відновити за допомогою** PowerShell. Ви можете відновити програму, яку потрібно відновити, за допомогою [Restore-AzureADDeletedApplication.](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
