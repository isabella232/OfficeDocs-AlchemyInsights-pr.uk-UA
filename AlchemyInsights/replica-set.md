---
title: Набір реплік
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
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714588"
---
# <a name="replica-set"></a>Набір реплік

AADDS також називають керованим доменом. Це насправді два контролери домену, які виконуються й підтримуються на внутрішньому сервері. Два ЦСК включають один основний DC і один реплікацію DC. Резервне копіювання в надбудові AADDS (керований домен) – це автоматизований процес, керований платформою Azure. У разі проблеми з керованим доменом, підтримка Azure може допомогти вам відновити роботу з резервної копії.

Ви створюєте набір реплік у віртуальній мережі. Кожна віртуальна мережа має бути в кожній іншій віртуальній мережі, де розміщено набір реплік керованого домену. Ця конфігурація створює топологію мережі сітки, яка підтримує реплікацію каталогів. Віртуальна мережа може підтримувати кілька наборів реплік, за умови, що кожний набір реплік перебуває в іншій віртуальній підмережі.

Докладні відомості про набір реплік наведено в статті [Набори реплік "концепції](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)".
