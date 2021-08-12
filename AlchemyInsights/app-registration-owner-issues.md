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
ms.openlocfilehash: cd7533f09ed8361e134b81979532cdebbf49971c54553a0172c7527f30e319bb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951154"
---
# <a name="app-registration-owner-issues"></a>Проблеми з реєстрацією в власників програм

Нижче наведено доступні способи додавання учасників як власників для реєстрації програм.

- Використання модуля Azure AD PowerShell

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    [Довідник: Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Використання Azure CLI – `az ad app owner add`

    Довідка: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)
- Використання MS Graph -

    Довідник: [додавання власника – microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Використання порталу Azure AD. Перейдіть до portal.azure.com [>](https://portal.azure.com/) Azure Active Directory > Реєстрації програм > Виберіть свою програму для > власників > Додати власників

**Не вдається переглянути програму на надписах реєстрації програм, навіть якщо ви – власник цієї програми?**

Власник програми не є адміністративною роллю. Якщо параметр [Обмежити доступ](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) до порталу адміністрування Azure AD ввімкнуто, переглядати програми на порталі реєстрації програм зможе лише адміністратор. Щоб власник зможе переглядати програми, вимкніть цей параметр (установіть значення "Ні") або призначте роль адміністратора власнику лише для конкретної програми. Однак для цього потрібно мати ліцензію на Azure AD Premium P2 та ввімкнути [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).
