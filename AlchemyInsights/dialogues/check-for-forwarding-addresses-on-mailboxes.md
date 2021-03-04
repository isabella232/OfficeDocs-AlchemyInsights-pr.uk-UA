---
title: Перевірка адрес для пересилання в поштових скриньках
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 17/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 1b0a6c8fe368196f2d1f9811aea895c2c024b2e6
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/03/2021
ms.locfileid: "50428160"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a>Перевірка адрес для пересилання в поштових скриньках

Іноді хакерам пересилаються повідомлення електронної пошти для користувачів, тому спочатку ми перевіряємо адреси для пересилання та правила в поштовій скриньці. Після цього ми перевіримо журнали аудиту. Ось як можна перевірити, чи є адреси для пересилання.

1. Виберіть **користувачів**  >  **активні користувачі**.
1. Виберіть користувача, обліковий запис якого було скомпрометовано.
1. У меню, що Відкриється, розгорніть розділ **Параметри пошти**, а потім натисніть кнопку **редагувати** для **пересилання електронної пошти**.
1. Видаліть усі адреси для пересилання, які не розпізнаються.