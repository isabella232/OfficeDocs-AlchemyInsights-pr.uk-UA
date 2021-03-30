---
title: Проблеми з реєстрацією в власників програм
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
- "9655"
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405325"
---
# <a name="app-registration-owner-issues"></a>Проблеми з реєстрацією в власників програм

Нижче наведено доступні способи додавання учасників як власників для реєстрації програм.

- Використання модуля Azure AD PowerShell

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    [Довідник: Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Використання Azure CLI – `az ad app owner add`

    Довідка: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)
- Використання MS Graph –

    Довідник: [додавання власника – Microsoft Graph 1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Використання порталу Azure AD. Перейдіть до portal.azure.com [>](https://portal.azure.com/) Azure Active Directory > Реєстрації програм > Виберіть свою програму для > власників > Додати власників

**Не вдається переглянути програму на надписах реєстрації програм, навіть якщо ви – власник цієї програми?**

Власник програми не є адміністративною роллю. Якщо параметр [Обмежити доступ](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) до порталу адміністрування Azure AD ввімкнуто, переглядати програми на порталі реєстрації програм зможе лише адміністратор. Щоб власник зможе переглядати програми, вимкніть цей параметр (установіть значення "Ні") або призначте роль адміністратора власнику лише для конкретної програми. Однак для цього потрібно мати ліцензію Azure AD Premium P2 та ввімкнути [керування привілейованими ідентичноями.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)
