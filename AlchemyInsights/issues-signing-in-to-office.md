---
title: Проблеми з входом в програми Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695308"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Пустий екран входу в програмах Microsoft 365

Щоб вирішити цю проблему, виконайте наведені нижче дії.
- Інсталюйте найновіші оновлення для [Windows](https://support.microsoft.com/help/4027667/windows-10-update) і [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Скидання параметрів браузера Internet Explorer: **Перехід до параметрів**  >  **Internet Options**  >  **Advanced**  >  браузера Internet**Explorer** (Зверніть увагу, що ви втратите додаткові параметри), а потім спробуйте ввійти в Office ще раз.
- Вимкнення засобу захисту від захисника Windows (WDAG) або будь-якого аналогічного брандмауера або антивірусної програми:
    1. На панелі керування виберіть пункт **програми**, а потім – **Увімкнути або вимкнути функції Windows**.
    2. Якщо ввімкнуто засіб захисту від захисника Windows, виконайте його вимкнення.<br/>
    **Примітка.** Можливо, знадобиться перезавантажити комп'ютер.
- Переконайтеся, що компонент Plug-in служби Microsoft. AAD. брокерсько [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) не блокує будь-яку програму або брандмауер/антивірусна програма.
- [Очищення облікових даних Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) за допомогою диспетчера облікових даних Windows.<br/>
    **Примітка.** Шляхи реєстру для Office 2016 змінилися на 16,0. (Приклад: \Software\microsoft\office\16.0\coment\identity\)

Щоб отримати докладніші відомості, ознайомтеся з [проблемами підключення під час входу в Office 2016 збірці 16.0.7967 у Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).