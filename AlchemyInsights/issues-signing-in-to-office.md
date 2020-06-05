---
title: Проблеми з входом у програми Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579922"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Порожній екран входу в Microsoft 365 Apps

Щоб вирішити цю проблему, спробуйте виконати такі дії:
- Інсталюйте останні оновлення для [Windows](https://support.microsoft.com/help/4027667/windows-10-update) і [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Скидання параметрів браузера Internet Explorer: перейдіть до розділу **засоби**  >  **Інтернет-параметри**  >  **Розширений**  >  **Скидання настройок браузера Internet Explorer** (Зауважте, що ви втратите користувацькі настройки), а потім спробуйте ввійти в Office знову.
- Вимкніть захисник програми Windows Defender (WDAG) або будь-який подібний брандмауер або антивірусна програма:
    1. На панелі керування перейдіть до **програми**, а потім виберіть пункт **Увімкнути або вимкнути засоби Windows**.
    2. Якщо активовано програму захисту захисника Windows, спробуйте вимкнути його.<br/>
    **Примітка:** Можливо, потрібно буде перезавантажити комп'ютер.
- Переконайтеся, що Microsoft. сад. брокера [сад WAM Plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) не блокується будь-який додаток або брандмауер/антивірусна програма.
- [Очистіть облікові дані Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) за допомогою диспетчера облікових даних Windows.<br/>
    **Примітка:** Шлях до реєстру для Office 2016 змінено на 16,0. (Напр.: \ програмне забезпеченя \mice\)

Щоб отримати додаткові відомості див [проблеми з підключенням після оновлення до Office 2016, створення 16.0.7967 на Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).