---
title: Визначити «вхідні» правилом активності в журнали аудиту
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1368
ms.assetid: ''
ms.openlocfilehash: f130846dd24cef81177934aa2a200c1056172d3f
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/07/2019
ms.locfileid: "34755058"
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
