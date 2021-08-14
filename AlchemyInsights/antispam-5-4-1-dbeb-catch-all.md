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
ms.openlocfilehash: e0e9b4fec0615943227f40043aeed842e8ee556c5916a59f65e79ce121ec9547
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932298"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Виправлення помилок доставки з кодом 550 5.4.1 Relay Access Denied

Ця проблема виникає під [час перевірки,](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) чи дійсна адреса електронної пошти для запобігання ненадійним викликам під час входу в мережу Microsoft. Спробуйте виконати такі дії:

1. Визначте, чи проблема характерна для всього домену або однієї адреси електронної пошти:
    - Увесь домен: іноді потрібно синхронізувати домен; спробуйте [вибрати для домену значення Внутрішній, а потім – на Повноважний.](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)
    - Одна адреса електронної пошти: іноді потрібно синхронізувати адресу; Змінення адреси проксі-сервера SMTP, а потім її повернення може допомогти.
2. Визначте, чи проблема характерна для групи або спільної папки. Для деяких типів об'єктів об'єкти, можливо, знадобиться створити Azure Active Directory.

Якщо вам потрібна додаткова допомога, надішліть запит на підтримку та вкажіть обсяг проблеми (зокрема тип об'єкта, на який ви надсилаєте повідомлення), щоб ми допомогли вам краще.