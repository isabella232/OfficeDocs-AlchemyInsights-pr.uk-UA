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
- "2560"
ms.openlocfilehash: 454000eafa6818f91e3c302cc69fbf252aae1107aa18904ac93a4756d4db642b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028061"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Виправлення помилок у Microsoft 365 "На жаль, інший обліковий запис із вашої організації вже ввійшли"

Щоб виправити цю помилку, спробуйте виконати наведені нижче дії.

- Видаліть усі робочі облікові записи, окрім відповідного, за допомогою Windows Настройки > **Access для роботи або навчання**.
- [Видаліть облікові Office, використовуючи](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) диспетчер Windows облікових даних.<br/>
    **Примітка.** Шляхи реєстру для Office 2016 змінено на 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Відкрийте файл програма Office виберіть Файловий **обліковий**  >  **запис**  >  **Вийти.** Потім увійдіть за допомогою облікового запису користувача з дійсною ліцензією. Докладні відомості про облікові записи в Office див. у [цій статті](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Для Mac див. статтю [Не вдається ввійти в програму Office 2016 для Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Докладні відомості див. в [розділі "На жаль,](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)інший обліковий запис вашої організації вже ввійшли на цьому комп'ютері" Office .