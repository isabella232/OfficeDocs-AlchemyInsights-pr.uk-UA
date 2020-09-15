---
title: Антиспам 5.4.1 DBEB Catch-All
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
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717382"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Вирішення проблем із доставкою для помилки з кодом 550 5.4.1-ретрансляцією відмовлено в доступі

Ця проблема виникає, [Якщо перевірити, чи є адреса електронної пошти дійсною, щоб запобігти bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) під час входу в мережу Microsoft. Виконайте наведені нижче дії.

1. Визначення того, чи ця проблема стосується всього домену або однієї адреси електронної пошти:
    - Увесь домен: іноді потрібно синхронізувати домен; Спробуйте [настроїти домен на внутрішній, а потім знову на важливий](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Єдина адреса електронної пошти: іноді потрібно синхронізувати адресу. Щоб змінити адресу проксі-сервера SMTP, а потім знову змінити його, може допомогти.
2. Визначення того, чи ця проблема стосується групи або спільної папки. Для деяких типів об'єктів, можливо, потрібно вручну створити в Лазурому Active Directory.

Якщо вам потрібна додаткова довідка, відкрийте квиток підтримки та вкажіть область цієї проблеми (включно з типом об'єкта, який ви надсилаєте), щоб ми могли краще допомогти вам.