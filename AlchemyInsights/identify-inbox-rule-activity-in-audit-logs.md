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
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1201a625948743cacfaa58410abeb4108ed2eb56
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539194"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Визначити «вхідні» правилом активності в журнали аудиту

Дає змогу аудиту журнал пошуку в Office 365 безпеки & центрі дотримання переглядати вхідні правила події (створення, редагування та видалення папки Вхідні правила).

1. Увійдіть до [Office 365 безпеки & центрі дотримання](https://protection.office.com/).

2. Перейти до **пошуку** > сторінку**пошуку журналу аудиту** .

3. Виберіть діапазон дат у полях **Дата початку** та **Дата завершення** .

4. За **Діяльність поштової скриньки Exchange**перевірте, чи **діяльність** поля має значення **Нью-InboxRule створити/змінити/увімкнути/вимкнути правило для вхідних повідомлень**.

5. Натисніть кнопку **Пошук**.

В результатах пошуку виберіть запис аудиту. У деталі спливаюче виберіть **Більше інформації**. Інформацію про параметри правило папки «Вхідні» відображається в області **параметрів** .

Докладніше перегляньте [Determining, якщо користувач створив правило для вхідних повідомлень](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
