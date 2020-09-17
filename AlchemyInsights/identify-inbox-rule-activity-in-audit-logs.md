---
title: Визначення дії правила для папки "Вхідні" в журналах аудиту
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779072"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Визначення дії правила для папки "Вхідні" в журналах аудиту

Ви можете використовувати пошук у журналі аудиту в центрі відповідності & безпеки Microsoft 365, щоб переглянути події правила для папки "Вхідні" (створення, змінення та видалення правил для папки "Вхідні").

1. Увійдіть у [центр відповідності & безпеки Microsoft 365](https://protection.office.com/).

2. Перейдіть на сторінку **Search**  >  **Пошук журналу аудиту** .

3. Виберіть діапазон дат у полях **Дата початку** та **Дата завершення** .

4. У розділі **дії поштової скриньки Exchange**переконайтеся, що в полі " **дії** " настроєно значення **"створити" або "змінити", щоб установити або вимкнути правило папки "Вхідні"**.

5. Натисніть кнопку **Пошук**.

У результатах виберіть запис аудиту. У розділі відомості про подробиці виберіть пункт **додаткові відомості**. Відомості про настройки правила для папки "Вхідні" відображаються в полі " **Параметри** ".

Докладні відомості наведено в статті [визначення того, чи користувач створив правило для папки "Вхідні"](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule) .
