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
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579886"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Виправлення програми Microsoft 365, "довірений платформи модуль не функціонує належним чином" повідомлення

Щоб виправити цю помилку, спробуйте виконати наведені нижче дії.

- Інсталюйте останні оновлення для [Windows](https://support.microsoft.com/help/4027667/windows-10-update) і [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Очистіть облікові дані Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) за допомогою диспетчера облікових даних Windows.<br/>
    **Примітка:** Шлях до реєстру для Office 2016 змінено на 16,0. (Напр.: \ програмне забезпеченя \mice\)
- Спробуйте [процес відновлення користувача](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) , щоб виправити НЕПОЛАДКИ модуля TPM.
- Встановіть EnableADAL = 0, виконавши наступні кроки:  
    1. Клацніть правою кнопкою миші кнопку Пуск Windows, виберіть **запустити**, введіть **Regedit**і натисніть кнопку **OK**.
    2. Виберіть **так** , щоб дозволити редактору реєстру вносити зміни до пристрою.
    3. У редакторі реєстру, додайте значення DWORD з **EnableADAL** параметр **0** , у розділі HKEY_CURRENT_USER \ програмне Забезпечена\mice\foot\16.0\ind\idat.

Щоб отримати додаткові відомості див [проблеми з підключенням після оновлення до Office 2016, створення 16.0.7967 на Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).