---
title: Політики збереження в Центрі адміністрування Exchange не працюють
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
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952249"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Політики збереження в Центрі адміністрування Exchange

Якщо ви хочете, щоб ми виконували автоматичні перевірки наведених нижче параметрів, натисніть кнопку "Назад" < – у верхній частині цієї сторінки, а потім введіть адресу електронної пошти користувача, який має проблеми з політиками збереження.

Якщо виникають проблеми з політиками збереження в Центрі адміністрування Exchange, які не застосовуються до поштових скриньок або елементів, які не переміщуються до архівної поштової скриньки, перевірте таке:

**Причини:**

- **Помічник із керованих** папок не обробив поштову скриньку користувача. Помічник із керованих папок намагається обробляти кожну поштову скриньку в хмарній організації один раз на сім днів.

  **Вирішення.** Запустіть помічник із керованих папок.

- **RetentionHold** **увімкнуто** в поштовій скриньці. Якщо поштову скриньку розміщено в Політиці збереження, політика збереження для поштової скриньки не оброблятимуться в цей час.

  **Вирішення.** Перевірте стан параметра утримання та оновіть його за потреби. Докладні відомості див. у [утримання поштової скриньки.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)
 
**Примітка.** Якщо розмір поштової скриньки менше 10 МБ, помічник із керованих папок не обробить поштову скриньку автоматично.
 
Докладні відомості про політики збереження в Центрі адміністрування Exchange див. у розділах:

- [Позначки та політики збереження](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Застосування політики збереження до поштових скриньок](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) або [додавання або видалення позначок збереження](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Визначення типу утримання, розміщеного в поштовій скриньці](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
