---
title: Користувацькі зображення й надалі відображатимуться Microsoft Teams організаційну діаграму
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13834"
- "9007457"
ms.openlocfilehash: be4c6feb55e6b7c4667566946d8d3640cc0ffb1d
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2021
ms.locfileid: "59422314"
---
# <a name="user-picture-still-appears-in-the-microsoft-teams-organization-chart"></a>Користувацькі зображення й надалі відображатимуться Microsoft Teams організаційну діаграму

Якщо в організації вимкнуто або видалено одного або кількох користувачів, а фотографія їхнього профілю все ще відображається на організаційній діаграмі, можливо, для параметра **ShowInAddressLists** установлено значення False: 

1. Перейдіть на Центр адміністрування Microsoft 365 > [Активні](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) користувачі та виберіть користувача з фотографією, яка все ще відображається. 
1. Виберіть вкладку **Пошта** та переконайтеся, що **для параметра Відображати в глобальному списку адрес** установлено значення **Ні.**

Якщо значення No (Ні) для  параметра **ShowInAddressLists** не працює, перевірте таке: 

- Можливо, користувач відображається в списку одержувачів у Exchange. Докладні відомості див. [в розділі Керування списками адрес у Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- Можливо, користувач відображається в списку адрес у Azure Active Directory. Докладні відомості див. [в дописі Set-AzureADUser.](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0) 