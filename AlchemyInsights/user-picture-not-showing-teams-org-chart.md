---
title: User picture not showing in Microsoft Teams organization chart
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/23/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12620"
- "9007457"
ms.openlocfilehash: 661b04913581ddd6650316298134ff9835ef3a90
ms.sourcegitcommit: 3986fa5377895cfc9fd98aca0739e599ebafb712
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/23/2021
ms.locfileid: "58792890"
---
# <a name="user-picture-not-showing-in-microsoft-teams-organization-chart"></a>User picture not showing in Microsoft Teams organization chart

Якщо на організаційній діаграмі відсутня фотографія профілю одного або кількох користувачів у вашій організації, можливо, для параметра **ShowInAddressLists** установлено значення **False:**

1. Перейдіть до Центр адміністрування Microsoft 365 > [**Активні**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)користувачі та виберіть користувача з відсутньою фотографією. 
1. Виберіть вкладку **Пошта** та переконайтеся, що **для параметра Відображати в глобальному списку адрес** установлено значення **Так.** 

Якщо значення **Yes (Так) для параметра ShowInAddressLists** не працює, перевірте таке: 

- Можливо, користувача приховано зі списку одержувачів у Exchange. Докладні відомості див. [в розділі Керування списками адрес у Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- Можливо, користувача приховано в списку адрес у Azure Active Directory. Докладні відомості див. [в дописі Set-AzureADUser.](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0) 
