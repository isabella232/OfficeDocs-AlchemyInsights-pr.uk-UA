---
title: Піктограма календаря не відображається в клієнті команд Microsoft
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: e28b1c8d5d0feef1a743c8527db424af4c205fe9
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583931"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a>Піктограма календаря не відображається в клієнті команд Microsoft

Вкладка " **календар** " в командах потребує доступу до поштової скриньки Exchange за допомогою веб-служб Exchange Web Services. Поштова скринька Exchange може перебувати в Інтернеті або в локальній мережі. Для користувачів Online, які не бачать вкладку **календар** , переконайтеся, що вони [ліцензовані для поштової скриньки Exchange Online, а поштова скринька увімкнена](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes). Якщо користувачі перебувають на локальному комп'ютері, потрібно підтвердити, що ваша Гібридна конфігурація здорова. Щоб вирішити проблему, скористайтеся [майстром гібридної конфігурації](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent). Зверніть увагу, що [для Teams необхідно інсталювати Exchange 2016 CU3 або новішої версії](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).

Щоб отримати докладніші відомості та вказівки з виправлення неполадок, перегляньте статтю [Виправлення неполадок із командами Microsoft і даними взаємодії сервера Exchange Server](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).
