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
- "2560"
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833096"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Виправлення помилок у програмах Microsoft 365 "На жаль, інший обліковий запис вашої організації вже ввійшли"

Щоб виправити цю помилку, спробуйте виконати наведені нижче дії.

- Видаліть усі робочі облікові записи, окрім відповідного, за допомогою параметрів Windows > **доступ до роботи або навчального закладу**.
- [Видаліть облікові дані Office за](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) допомогою диспетчера облікових даних Windows.<br/>
    **Примітка.** Шляхи реєстру для Пакета Office 2016 змінено на 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Відкрийте програму Office і виберіть **Вийти** з  >    >  **облікового запису файлу**. Потім увійдіть за допомогою облікового запису користувача з дійсною ліцензією. Докладні відомості див. в статті [Облікові записи в Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Для Mac див. статтю [Не вдається ввійти в програму Office 2016 для Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Докладні відомості див. в розділі "На жаль, інший обліковий запис вашої організації вже ввійшли на [цьому комп'ютері" в Office.](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)