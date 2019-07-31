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
- "2559"
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938384"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Фіксація Office apps "модуля TPM надійних ваш комп'ютер працює неправильно" повідомлення

Щоб виправити цю помилку, спробуйте наступне:

- Інсталюйте останні оновлення для [Windows](https://support.microsoft.com/help/4027667/windows-10-update) і [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Ясно Office облікові дані](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) за допомогою диспетчера облікових даних Windows.<br/>
    **Примітка:** 16,0 змінили реєстру доріжки для офісу 2016. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Повторіть [процес відновлення користувача](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) виправити надійні платформи модуля TPM невдач.
- Встановити в EnableADAL = 0, виконавши наведені нижче дії:  
    1. Клацніть правою кнопкою миші кнопку Windows Пуск, виберіть **виконати**, введіть **regedit**а потім виберіть **ОК**.
    2. Виберіть, **так** щоб дозволити редактор реєстру для внесення змін до пристрою.
    3. У редакторі реєстру додайте значення DWORD з **EnableADAL** з значення **0** під HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Докладніше перегляньте [підключення проблеми у входу після оновлення до Office 2016 побудувати 16.0.7967 на версії 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).