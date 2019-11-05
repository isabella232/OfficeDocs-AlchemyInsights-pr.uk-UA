---
title: Антиспам 5.4.1 DBEB зловити-все
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: 4a56cfe74d8940e53a316d3bcc3809e8666c2e37
ms.sourcegitcommit: a8945ab0008f138b2992175b0640e78a505d29e1
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 11/04/2019
ms.locfileid: "37964367"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Вирішення проблем із доставкою код помилки 550 5.4.1 ретранслятор доступ заборонено

Ця проблема виникає під час [перевірки, щоб побачити, якщо адреса електронної пошти дійсний для запобігання](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) під час переходу до мережі Office 365. Спробуйте виконати такі дії:

1. Визначте, чи проблема стосується всього домену або одну адресу електронної пошти:
    - Увесь домен: інколи потрібно синхронізувати домен; Спробуйте [настроїти домен на внутрішній, а потім повернутися до основного](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
     - Єдина адреса електронної пошти: іноді адреса повинна бути синхронізована; зміна адреси SMTP-проксі-сервера, а потім змінити його назад може допомогти.
2. Визначте, чи проблема специфічна для групи або спільних папок. Для деяких типів об'єктів, можливо, доведеться вручну створити в Azure Active Directory.

Якщо вам потрібна додаткова допомога, будь ласка, відкрийте квиток підтримки і вкажіть сферу цього питання (включаємо тип об'єкту, який ви посилаєте), щоб ми могли допомогти вам краще.