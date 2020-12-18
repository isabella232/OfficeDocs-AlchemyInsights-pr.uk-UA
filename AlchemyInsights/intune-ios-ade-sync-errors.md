---
title: Помилки синхронізації автоматичної реєстрації пристрою в Apple
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
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714971"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Помилки синхронізації автоматичної реєстрації пристрою в Apple

"Виявлено, що у вас є один або кілька маркерів ADE/DEP, які знаходяться в стані помилки. Доки стан помилки не буде вирішено для кожного відповідного маркера, функція ADE не працюватиме для одних і тих самих ".

Ця помилка може виявлятися кількома способами, зокрема:

1. Пристрої можуть не синхронізуватися з ABM/ASM для Inune
2. Можливо, не вдається отримати відповідні завдання для реєстрації
3. Можливо, для пристроїв не вдалося завершити реєстрацію в "ADE"

Перевірте, чи повідомлення про помилку синхронізації відобразилось в консолі Inune в розділі **пристрої, > записатися на пристрої > програми реєстрації в програмі Apple >** , а також Перегляньте наведені нижче документи, щоб переглянути потенційні виправлення.

[Помилки синхронізації АБМ/АНМ для маркерів реєстрації для iOS/iPadOS і macOS для автоматичних пристроїв](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
