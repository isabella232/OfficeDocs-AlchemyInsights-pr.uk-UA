---
title: Помилки автоматичної синхронізації пристрою Apple
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
ms.openlocfilehash: 1664a26b313c4a38c9c6d78cdb89997749ba175fd3dd72f278e99bbd50b0ee84
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013769"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Помилки автоматичної синхронізації пристрою Apple

"Ми виявили, що у вас є один або кілька маркерів ADE/DEP, які переносяться до стану помилки. Функціональні можливості ADE не працюватимуть належним чином, доки стан помилки не буде вирішено для кожного відповідного маркера.

Ця помилка може проявитися різними способами, зокрема:

1. Пристрої можуть не синхронізуватися з ABM/ASM в Intune
2. Можливо, не вдалось виконати призначення профілю входу
3. Можливо, пристрої не завершено, можливо, не завершено підписку на ADE

Перевірте, чи не повідомлено про помилку синхронізації в консолі Intune у розділі Пристрої > реєстрації пристроїв і > маркери реєстрації Apple > маркери **програми реєстрації.**

Одна з найпоширеніших причин помилки синхронізації – завершення терміну дії поточного маркера. У багатьох випадках проблему вирішує поновлення відповідного маркера.

Якщо термін дії одного або кількох маркерів минув, перегляньте наведену нижче документацію, щоб дізнатися, як їх поновити.

[Подовження маркера автоматизованої безпеки пристрою](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Крім того, ви можете переглянути наведену нижче документацію, щоб дізнатися про можливі способи усунення інших помилок, які можуть викликати помилки синхронізації маркерів.

[Помилки синхронізації ABM або ASM для iOS/iPadOS і маркерів автоматичного розгортання пристроїв для macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[Помилки синхронізації ABM або ASM для iOS/iPadOS і маркерів автоматичного розгортання пристроїв для macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
