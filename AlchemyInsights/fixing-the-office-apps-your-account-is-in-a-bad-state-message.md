---
title: Фіксація програм Office обліковий запис перебуває в повідомленні поганий стан
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969913"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a>Виправлення помилок програм Office "ваш обліковий запис перебуває в поганому стані"

Щоб виправити цю помилку, спробуйте на проблемному комп'ютері такі параметри:

- Відкрийте програму Office **, виберіть** > **обліковий запис** > ,**вийдіть із всіх облікових записів**. Увійдіть знову, використовуючи обліковий запис користувача з дійсною ліцензією. Докладні відомості наведено [в облікових записах в Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Очистіть облікові дані Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) за допомогою диспетчера облікових даних Windows.<br>
  **Примітка:** Шлях до реєстру для Office 2016 змінено на 16,0. Наприклад, \ програмне Забезпечена\micfr\fore\16.0\ \ \ \
- На проблемному комп'ютері встановіть EnableADAL = 0, виконавши такі дії:  
     1. Клацніть правою кнопкою миші кнопку Windows і виберіть **запустити**. У полі " **Відкрити** " введіть **Regedit**і виберіть **"OK"**.
     2. Виберіть **так** , коли буде запропоновано дозволити редактору реєстру вносити зміни до пристрою.
    3. У редакторі реєстру, додайте значення DWORD з EnableADAL параметр 0, у розділі HKEY_CURRENT_USER \ програмне Забезпеченми\mice\foot\16.0\ind\idt.
- Якщо сталася помилка під час підключення до Office 365 за допомогою Office 2013, [Увімкніть сучасних автентифікації](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) для клієнта Office.

Щоб отримати додаткові відомості, Дізнайтеся, [як вирішити проблеми, не-браузер застосунків, які не вдається ввійти до Office 365, Azure або InTune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

