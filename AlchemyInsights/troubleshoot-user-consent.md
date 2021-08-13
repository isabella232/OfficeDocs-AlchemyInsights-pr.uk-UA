---
title: Виправлення неполадок, пов'язаних із згодою користувача
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
- "9004353"
- "7785"
ms.openlocfilehash: db784c133fec554604ad09f5b27941879d97ff238f926ff6338d0f3b7c3c4105
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007919"
---
# <a name="troubleshoot-user-consent"></a>Виправлення неполадок, пов'язаних із згодою користувача

1. Ви можете налаштувати спосіб отримання згоди кінцевих користувачів на програми через портал Azure або PowerShell. Докладні [відомості див. в розділі](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) Параметри згоди користувача.
1. Адміністратор також може надати згоду [Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) корпорації Майкрософт від імені одного користувача. Докладні відомості [див. в відео Отримання](https://docs.microsoft.com/graph/auth-v2-user)доступу від імені користувача.
1. [Помилки згоди користувачів.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)У цій статті описано помилки, які можуть виникнути під час згоди програми. Якщо ви виправляєте неочікувані запити на згоду, які не містять жодних повідомлень про помилку, див. номери Сценарії [автентифікації для Azure AD.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)