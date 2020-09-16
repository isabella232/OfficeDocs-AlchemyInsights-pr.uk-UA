---
title: Виправлення програм Microsoft 365, які обліковий запис має поганий стан повідомлення
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
- "2558"
- "9000571"
ms.openlocfilehash: ec529291ec9406eba9dc2b0f2cc7a93c77fa3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744566"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Помилка фіксації програм Microsoft 365 "ваш обліковий запис перебуває в поганій державі"

Щоб виправити цю помилку, виконайте наведені нижче дії на ураженого комп'ютера.

- Відкрийте програму Office, виберіть пункт **File**  >  **обліковий запис**файлу, щоб  >  **вийти з усіх облікових записів**. Увійдіть знову, використовуючи обліковий запис користувача з дійсною ліцензією. Докладні відомості див. в статті [Облікові записи в Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Очищення облікових даних Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) за допомогою диспетчера облікових даних Windows.<br>
  **Примітка.** Шляхи реєстру для Office 2016 змінилися на 16,0. Наприклад, \Software\Microsoft\Office\16.0\Common\Identity\
- Якщо помилка виникає під час підключення до Office 365 за допомогою служби Office 2013, [Увімкніть сучасну автентифікацію](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) для клієнта Office.

Щоб отримати докладні відомості, Дізнайтеся, [як усунути неполадки, які не є браузерами, які не можуть входити в Microsoft 365, Azure або InTune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

