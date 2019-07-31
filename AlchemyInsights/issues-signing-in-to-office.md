---
title: Питання, ввійшовши до служби Office
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
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938383"
---
# <a name="blank-sign-in-screen-in-office-apps"></a>Пустий екрана входу в Office apps

Щоб виправити цю проблему, спробуйте наступне:
- Інсталюйте останні оновлення для [Windows](https://support.microsoft.com/help/4027667/windows-10-update) і [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Скинути параметри Internet Explorer: Заходимо **інструменти** > **Властивості браузера** > **Додатково** > **Скидання настройок Internet Explorer** (Зверніть увагу, що вам буде втрачено користувацькі настройки) після чого спробуйте ввійти до офісу знову.
- Відключити будь-які аналогічні брандмауера або антивірусної програми або гвардії застосунок Windows Defender (WDAG):
    1. На панелі керування перейдіть до **програми**а потім виберіть **засоби Windows увімкнути або вимкнути**.
    2. Якщо активовано Windows Defender застосування гвардії, відключіть його.<br/>
    **Примітка:** Може знадобитися перезавантаження комп'ютера.
- Переконайтеся, що Microsoft.AAD.BrokerPlugin [Сад WAM плагін](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) не час заблоковано всі програми або брандмауер/anti-virus програми.
- [Ясно Office облікові дані](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) за допомогою диспетчера облікових даних Windows.<br/>
    **Примітка:** 16,0 змінили реєстру доріжки для офісу 2016. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Докладніше перегляньте [підключення проблеми у входу після оновлення до Office 2016 побудувати 16.0.7967 на версії 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).