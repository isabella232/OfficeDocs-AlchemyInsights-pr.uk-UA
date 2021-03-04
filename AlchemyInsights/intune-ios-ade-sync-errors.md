---
title: Помилки синхронізації автоматичної реєстрації пристрою в Apple
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
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448943"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Помилки синхронізації автоматичної реєстрації пристрою в Apple

"Виявлено, що у вас є один або кілька маркерів ADE/DEP, які знаходяться в стані помилки. Доки стан помилки не буде вирішено для кожного відповідного маркера, функція ADE не працюватиме належним чином. ".

Ця помилка може виявлятися кількома способами, зокрема:

1. Пристрої можуть не синхронізуватися з ABM/ASM для Inune
2. Можливо, не вдається отримати відповідні завдання для реєстрації
3. Можливо, для пристроїв не вдалося завершити реєстрацію в "ADE"

Перевірте, чи повідомлення про помилку синхронізації повідомляється в консолі Inune в розділі **пристрої, > записатися на пристрої > програми реєстрації в програмі Apple > маркери для реєстрації**.

Однією з найпоширеніших причин помилки синхронізації є термін дії поточного маркера. У багатьох випадках відновлення ураженого маркера вирішить проблему.

Якщо термін дії одного або кількох маркерів минув, ознайомтеся з наведеною нижче документацією, щоб допомогти вам поновити їх відповідно до таких потреб:

[Поновлення маркера реєстрації автоматичного пристрою](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Крім того, можна переглянути наведені нижче документи, щоб переглянути потенційні помилки для інших помилок, які призводять до помилок синхронізації маркерів.

[Помилки синхронізації АБМ/АНМ для маркерів реєстрації для iOS/iPadOS і macOS для автоматичних пристроїв](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[Помилки синхронізації АБМ/АНМ для маркерів реєстрації для iOS/iPadOS і macOS для автоматичних пристроїв](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
