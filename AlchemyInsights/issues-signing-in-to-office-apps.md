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
- "2560"
ms.openlocfilehash: 7d2cfd437bb55804c3b9263428833c10d5caaa47
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695344"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Виправлення програм Microsoft 365 "на жаль, ще один обліковий запис у вашій організації вже підписано" повідомлення

Щоб виправити цю помилку, спробуйте виконати наведені нижче дії.

- Видаліть усі робочі облікові записи, крім ураженого облікового запису, використовуючи параметри Windows, > **доступ до роботи або навчального закладу**.
- [Очищення облікових даних Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) за допомогою диспетчера облікових даних Windows.<br/>
    **Примітка.** Шляхи реєстру для Office 2016 змінилися на 16,0. (Приклад: \Software\microsoft\office\16.0\coment\identity\)
- Відкрийте програму Office, виберіть пункт **File**"  >  **обліковий запис**файлу"  >  **Sign Out**. Після цього увійдіть за допомогою облікового запису користувача з дійсним ліцензією. Докладні відомості див. в статті [Облікові записи в Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Для Mac див. статтю [Не вдається ввійти в програму Office 2016 для Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Щоб отримати докладніші відомості, у [службі Office вже ввійшли інші облікові записи з організації на цьому комп'ютері](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).