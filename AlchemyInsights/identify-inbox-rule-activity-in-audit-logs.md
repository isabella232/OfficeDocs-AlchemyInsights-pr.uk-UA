---
title: Визначити «вхідні» правилом активності в журнали аудиту
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1368
ms.assetid: ''
ms.openlocfilehash: 9339d9c58056f568dc994b75bffe39f2c8bbdd34
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/23/2019
ms.locfileid: "32417267"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Визначити «вхідні» правилом активності в журнали аудиту

За допомогою пошуку журналу аудиту безпеки & відповідно центр для перегляду папки «Вхідні» правилом події (створення, редагування та видалення папки Вхідні правила).

1. Увійдіть до [Office 365 безпеки & відповідно центр](https://protection.office.com/)

2. Натисніть кнопку **Пошук та розслідування** та виберіть **Пошук журналу аудиту**.

3. Виберіть діапазон дат у полях **Дата початку** та **Дата завершення** .

4. За **Діяльність поштової скриньки Exchange**перевірте, чи **діяльність** поля має значення **Нью-InboxRule створити/змінити/увімкнути/вимкнути правило для вхідних повідомлень**.

5. Натисніть кнопку **Пошук**.

В результатах пошуку виберіть запис аудиту. У деталі спливаюче виберіть **Більше інформації**. Інформацію про параметри правило папки «Вхідні» відображається в області **параметрів** .

Докладніше перегляньте [Determining, якщо користувач створив правило для вхідних повідомлень](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
