---
title: Проблеми з входом у програми Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833060"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Пустий екран входу в програмах Microsoft 365

Щоб вирішити цю проблему, спробуйте зробити ось що:
- Інсталюйте останні оновлення [для Windows](https://support.microsoft.com/help/4027667/windows-10-update) і [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- Скидання параметрів Internet Explorer: перейдіть до меню Знаряддя Властивості браузера Додаткові параметри скидання  >    >    >  **настройок Internet Explorer** (зверніть увагу, що ви втратите власні настройки), а потім спробуйте ввійти в Office ще раз.
- Вимкніть Засіб захисту програм для Захисника Windows (WDAG) або будь-який подібний брандмауер чи антивірусну програму:
    1. На Панелі керування відкрийте меню **Програми**, а потім виберіть елемент **Увімкнути або вимкнути компоненти Windows**.
    2. Якщо засіб захисту програм для Захисника Windows увімкнуто, спробуйте вимкнути його.<br/>
    **Примітка.** Можливо, знадобиться перезавантажити комп'ютер.
- Переконайтеся, що компонент plug-in AAD.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) не блокується жодною програмою, брандмауером або антивірусним програмою.
- [Видаліть облікові дані Office за](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) допомогою диспетчера облікових даних Windows.<br/>
    **Примітка.** Шляхи реєстру для Пакета Office 2016 змінено на 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Докладні відомості див. в статтях Проблеми з підключенням після входу в систему після оновлення [до збірки Office 2016 16.0.7967 у Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)