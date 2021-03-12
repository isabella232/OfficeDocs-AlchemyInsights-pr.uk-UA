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
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709127"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Виправлення повідомлень програми Microsoft 365 "модуль надійної платформи на комп'ютері не функціонує

Щоб виправити цю помилку, спробуйте виконати наведені нижче дії.

- Інсталюйте найновіші оновлення для [Windows](https://support.microsoft.com/help/4027667/windows-10-update) і [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Очищення облікових даних Office](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) за допомогою диспетчера облікових даних Windows.<br/>
    **Примітка.** Шляхи реєстру для Office 2016 змінилися на 16,0. (Приклад: \Software\microsoft\office\16.0\coment\identity\)
- Випробуйте [процес відновлення користувача](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) , щоб виправити помилки модуля TPM.
- Установіть значення EnableADAL = 0, виконавши наведені нижче дії.  
    1. Клацніть правою кнопкою миші кнопку Windows Пуск, виберіть команду **виконати**, введіть **Regedit** і натисніть **кнопку OK**.
    2. Натисніть кнопку " **так** ", щоб дозволити редактору реєстру вносити зміни до вашого пристрою.
    3. У редакторі реєстру додайте значення DWORD в **EnableADAL** з параметром **0** під HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Щоб отримати докладніші відомості, ознайомтеся з [проблемами підключення під час входу в Office 2016 збірці 16.0.7967 у Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).