---
title: Змінення Microsoft EDGE за допомогою змінних каталогів даних, а не жорстко
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "9003873"
- "6926"
ms.openlocfilehash: 5c40aa1d7f61fbd2842839a5839899af8ab439f2
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679156"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a>Змінення Microsoft EDGE за допомогою змінних каталогів даних, а не жорстко

Наприклад, у Windows для зберігання даних профілю в розділі Локальні дані програми користувача, а не в розташуванні за замовчуванням, установіть політику **UserDataDir** to **$ {local_app_data} \Edge\Profile**. 

Докладні відомості можна знайти в статті [створення змінних каталогів даних для користувачів служби Microsoft EDGE](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars).