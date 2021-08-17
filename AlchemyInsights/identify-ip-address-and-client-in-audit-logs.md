---
title: Визначення IP-адреси та клієнта в контрольних журналах
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
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 080b3df3934781ebf0d0cd5243787bf6975fc5f123b5b1593c0b6d9ada4eae5d
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/11/2021
ms.locfileid: "57887521"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Визначення IP-адреси та клієнта в контрольних журналах

IP-адреса, яка відповідає дії користувача або Microsoft 365 відображається в контрольних журналах. Крім того, записуються відомості про клієнта. Нижче описано, як визначити таку інформацію.

1. Увійдіть [у Центр Microsoft 365 відповідності.](https://protection.office.com/)

2. Перейдіть на сторінку **Пошук**  >  **у контрольного журналу.**

   Якщо вас цікавить певна діяльність, виберіть її зі списку **Дії.** Якщо ні, для вибраного користувача буде повернуто всі дії (за замовчуванням).

   **Примітка.** Певні дії можуть бути недоступні в **меню Дії.** проте ці елементи буде повернуто, якщо вибрано Показати результати для **всіх** дій (за замовчуванням).

3. Укажіть ім'я користувача **в полі** Користувачі, виберіть відповідний діапазон дат для дії, а потім натисніть **кнопку Пошук**.

У результатах IP-адресу для цієї дії можна переглянути в області результатів. Виберіть запис аудиту, щоб  переглянути докладні відомості в розгортці докладних відомостей (наприклад, Клієнт, користувач, який виконав дію тощо).

Докладні відомості див. в статтях Пошук IP-адреси комп'ютера, що використовується для доступу до [злама облікового запису.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)
