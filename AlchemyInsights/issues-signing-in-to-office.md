---
title: Проблеми з входом у Microsoft 365 програми
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
ms.openlocfilehash: 7a8a0b68fc211e99b22e857d51d1de54e53a69357f75a0c60b1e83078cd5b27f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088057"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Пустий екран входу в Microsoft 365 програми

Щоб вирішити цю проблему, спробуйте зробити ось що:
- Інсталюйте останні оновлення [для Windows](https://support.microsoft.com/help/4027667/windows-10-update) і [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Скидання параметрів Internet Explorer: перейдіть до меню Знаряддя Параметри браузера Додатково Скинути параметри  >    >    >  **Internet Explorer Настройки** (зверніть увагу, що ви втратите користувацькі настройки) і спробуйте ввійти, щоб Office ще раз.
- Вимкніть Засіб захисту програм для Захисника Windows (WDAG) або будь-який схожий брандмауер чи антивірусну програму:
    1. На Панелі керування відкрийте меню **Програми**, а потім виберіть пункт Windows **функції.**.
    2. Якщо Засіб захисту програм для Захисника Windows, спробуйте вимкнути його.<br/>
    **Примітка.** Можливо, знадобиться перезавантажити комп'ютер.
- Переконайтеся, що компонент plug-in AAD.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) не блокується жодною програмою, брандмауером або антивірусним програмою.
- [Видаліть облікові Office, використовуючи](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) диспетчер Windows облікових даних.<br/>
    **Примітка.** Шляхи реєстру для Office 2016 змінено на 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Докладні відомості див. в цій Office [16.0.7967](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)в Windows 10.