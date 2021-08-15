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
- "2559"
ms.openlocfilehash: b0789a54f48b2850c1dad8651a8209449c805784bea96799f05e67c4bc43fdb0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986912"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Виправлення помилок у Microsoft 365 "Модуль надійної платформи комп'ютера працює неправильно"

Щоб виправити цю помилку, спробуйте виконати наведені нижче дії.

- Інсталюйте останні оновлення [для Windows](https://support.microsoft.com/help/4027667/windows-10-update) і [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Видаліть облікові Office, використовуючи](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) диспетчер Windows облікових даних.<br/>
    **Примітка.** Шляхи реєстру для Office 2016 змінено на 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Спробуйте відновити [користувача, щоб](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) виправити помилки модуля TPM.
- Установіть значення EnableADAL = 0, як описано нижче.  
    1. Клацніть правою кнопкою миші Windows кнопку Пуск, виберіть **виконати**, введіть **regedit** і натисніть кнопку **OK.**
    2. Виберіть **Так,** щоб дозволити редактору реєстру вносити зміни на пристрої.
    3. У редакторі реєстру додайте значення DWORD **параметра EnableADAL** із **значенням 0** у розділі HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Докладні відомості див. в цій Office [16.0.7967](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)в Windows 10.