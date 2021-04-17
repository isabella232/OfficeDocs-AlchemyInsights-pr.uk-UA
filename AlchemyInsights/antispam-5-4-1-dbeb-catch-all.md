---
title: AntiSpam 5.4.1 DBEB catch-all
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
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821468"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Виправлення помилок доставки з кодом 550 5.4.1 Relay Access Denied

Ця проблема виникає під [час перевірки,](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) чи дійсна адреса електронної пошти для запобігання ненадійним викликам під час входу в мережу Microsoft. Спробуйте виконати такі дії:

1. Визначте, чи проблема характерна для всього домену або однієї адреси електронної пошти:
    - Увесь домен: іноді потрібно синхронізувати домен; спробуйте [вибрати для домену значення Внутрішній, а потім – на Повноважний.](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)
    - Одна адреса електронної пошти: іноді потрібно синхронізувати адресу; Змінення адреси проксі-сервера SMTP, а потім її повернення може допомогти.
2. Визначте, чи проблема характерна для групи або спільної папки. Для деяких типів об'єктів в Azure Active Directory може знадобитися вручну створити об'єкти.

Якщо вам потрібна додаткова допомога, надішліть запит на підтримку та вкажіть обсяг проблеми (зокрема тип об'єкта, на який ви надсилаєте повідомлення), щоб ми допомогли вам краще.