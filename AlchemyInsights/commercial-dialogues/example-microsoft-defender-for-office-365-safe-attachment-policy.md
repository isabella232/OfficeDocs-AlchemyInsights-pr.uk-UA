---
title: Приклад політики вкладення для Office 365 Сейф Microsoft Defender
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 7294be81a24fa61a92367bae304798a333cb916c8718e28b1a87314c15ef6c8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988316"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Приклад політики вкладення для Office 365 Сейф Microsoft Defender

Ці параметри дають  змогу ввімкнути політику під назвою "Без затримки", яка миттєво доставляє повідомлення, а потім повторно підставляє вкладення після їх сканування.

- **Ім'я:** без затримок
- **Опис.** Доставляє повідомлення відразу та повторно підставляє вкладення після сканування.
- **Відповідь.** Виберіть параметр **динамічної доставки.** Докладні відомості див. в [цій Сейф.](https://go.microsoft.com/fwlink/?linkid=2092328)
- **Розділ Переспрямування** вкладення: виберіть параметр Увімкнути переспрямування **,** а потім введіть адресу електронної пошти глобального адміністратора Microsoft 365, адміністратора безпеки або аналітика безпеки, який вивчає зловмисні вкладення.
- **Розділ Застосовано** до. **Виберіть елемент Доменом одержувача** є , а потім виберіть свій домен. Виберіть **додати**, а потім натисніть **кнопку OK**. Завершивши, натисніть кнопку **Зберегти**.

Докладні відомості див. [в статті Сейф вкладення в Захиснику Microsoft Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).
