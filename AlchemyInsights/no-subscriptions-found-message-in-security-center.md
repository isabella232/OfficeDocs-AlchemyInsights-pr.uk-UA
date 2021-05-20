---
title: Повідомлення про те, що передплати не знайдено в Центрі безпеки
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544129"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a>Повідомлення про те, що передплати не знайдено в Центрі безпеки

Якщо під час доступу Центр безпеки для Microsoft Defender з'являється повідомлення "Передплати не знайдено", це означає, що Azure Active Directory (AAD) для входу користувача на портал не має ліцензії ВВП для Microsoft Defender.  

Ліцензії Windows E5 Office E5 – це окремі ліцензії.

Відкрийте інцидент підтримки, якщо ліцензію придбано, але не підготовлено для цього екземпляра AAD. У вас є: <br/>
-   Можлива проблема з підготовкою ліцензій.<br/>
-   Ви ненавмисно підготували ліцензію на іншу службу Microsoft AAD, ніж та, що використовується для автентифікації в службі.