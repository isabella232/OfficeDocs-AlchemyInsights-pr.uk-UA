---
title: Виправлення неполадок із згодою користувача
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
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901625"
---
# <a name="troubleshoot-user-consent"></a>Виправлення неполадок із згодою користувача

1. Ви можете налаштувати спосіб згоди користувачів на програми за допомогою порталу "Лазурний" або PowerShell. Щоб отримати докладніші відомості, ознайомтеся з [настройками згоди користувача](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) .
1. Адміністратор також може використовувати [Microsoft GRAPH API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) , щоб надати згоду на делеговані дозволи від імені одного користувача. Докладні відомості наведено в статті [отримати доступ від імені користувача](https://docs.microsoft.com/graph/auth-v2-user).
1. [Помилки згоди користувачів](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): у цій статті розглядаються помилки, які можуть виникати під час процесу згоди на програму. Якщо ви не маєте права на запити про неочікувані згоди, які не містять повідомлень про помилки, ознайомтеся [з сценаріями автентифікації для Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).