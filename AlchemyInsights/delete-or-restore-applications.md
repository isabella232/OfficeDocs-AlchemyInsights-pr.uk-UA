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
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015022"
---
# <a name="delete-or-restore-applications"></a>Видалення або відновлення програм

**Щоб видалити програму зі свого клієнта Azure AD**, виконайте наведені нижче дії.

1. На **порталі Лазурне AD** виберіть елемент **корпоративні програми**. Потім знайдіть і виберіть програму, яку потрібно видалити.
2. У розділі **керування** в області ліворуч виберіть **Властивості**.
3. Натисніть кнопку **Видалити**, а потім натисніть кнопку **так** , щоб підтвердити видалення програми зі свого клієнта Azure AD.

Докладні відомості про видалення програми наведено в статті [QuickStart: видалення програми зі свого клієнта Azure Active Directory (AZURE AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).

У PowerShell цей командлет DELETE [-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) видаляє конфігурації проксі-сервера програми з певної програми в лазуровому Active Directory та може видалити програму повністю, якщо це вказано.

Ви можете **відновити видалену програму** за допомогою PowerShell. Після того, як програма, яку потрібно відновити, була виявлена, її можна відновити за допомогою функції [відновлення – AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
