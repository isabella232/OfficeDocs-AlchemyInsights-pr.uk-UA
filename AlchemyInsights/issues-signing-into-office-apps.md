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
- "2559"
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695200"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Виправлення повідомлень програми Microsoft 365 "модуль надійної платформи на комп'ютері не функціонує

Щоб виправити цю помилку, спробуйте виконати наведені нижче дії.

- Інсталюйте найновіші оновлення для [Windows](https://support.microsoft.com/help/4027667/windows-10-update) і [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Очищення облікових даних Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) за допомогою диспетчера облікових даних Windows.<br/>
    **Примітка.** Шляхи реєстру для Office 2016 змінилися на 16,0. (Приклад: \Software\microsoft\office\16.0\coment\identity\)
- Випробуйте [процес відновлення користувача](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) , щоб виправити помилки модуля TPM.
- Установіть значення EnableADAL = 0, виконавши наведені нижче дії.  
    1. Клацніть правою кнопкою миші кнопку Windows Пуск, виберіть команду **виконати**, введіть **Regedit**і натисніть **кнопку OK**.
    2. Натисніть кнопку " **так** ", щоб дозволити редактору реєстру вносити зміни до вашого пристрою.
    3. У редакторі реєстру додайте значення DWORD в **EnableADAL** із параметром **0** під HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.

Щоб отримати докладніші відомості, ознайомтеся з [проблемами підключення під час входу в Office 2016 збірці 16.0.7967 у Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).