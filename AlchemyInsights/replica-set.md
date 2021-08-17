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
ms.openlocfilehash: 45cf530c3258fa3c7008c3e8251fdb7b74be6911d0487f58c5ce2530e25ca282
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54110701"
---
# <a name="replica-set"></a>Набір реплік

AADDS також називається керованим доменом. Це насправді два контролери доменів, які запускають і об зберігаються сервером. Два типи DC містять одну головну копію (DC) і один тип реплікації (DC). Резервне копіювання в AADDS (керованому домені) – це автоматизований процес, який керує платформою Azure. Якщо виникне проблема з вашим керованим доменом, служба підтримки Azure може допомогти вам відновити його з резервної копії.

Кожний набір репліки створюється у віртуальній мережі. Кожну віртуальну мережу потрібно одно одноразової віртуальній мережі, яка розміщує набір репліки керованого домену. У цій конфігурації створюється топологія мережі-сітки, яка підтримує реплікацію каталогів. Віртуальна мережа може підтримувати кілька наборів реплік за умови, що кожен набір репліки розташовано в іншій віртуальній підмережі.

Докладні відомості про набір реплік див. в [цьому наборі.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)
