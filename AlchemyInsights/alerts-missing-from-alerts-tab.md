---
title: Оповіщення, відсутні на вкладці "Оповіщення"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12732"
ms.openlocfilehash: 9fbd9a32e40d858f0ba49931c723a824478aaa12
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/16/2021
ms.locfileid: "58454962"
---
# <a name="alerts-missing-from-alerts-tab"></a>Оповіщення, відсутні на вкладці "Оповіщення"

**Вкладка** "Оповіщення" працює на основі політик налаштування та активації з порталу керування програмами клієнта. Крім того, потрібно активувати готові політики програми, щоб сигнали стікали на **вкладку Оповіщення.** 

Переконайтеся, що оповіщення створено:

1. Перейдіть до політик керування програмами [та](https://compliance.microsoft.com/m365appprotection?viewid=policies) переконайтеся, що ви створили принаймні одну політику "Активні" або "Аудит".

1. Виберіть політику, а потім  в області виліт виберіть Редагувати. 

1. Перевірте конфігурацію політики, щоб переконатися, що оповіщення має бути створено на основі події політики, ініційованої понад 24 годинами тому.

Докладні відомості про оповіщення в управлінні програмами див. в цій [сторінці.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-detect-remediate-get-started)