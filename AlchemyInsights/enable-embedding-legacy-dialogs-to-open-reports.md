---
title: Увімкнення вбудовування застарілих діалогових вікон для відкриття звітів
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814285"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Увімкнення вбудовування застарілих діалогових вікон для відкриття звітів

**Ознака**

Користувачам не вдається відкрити звіти. "Сталася помилка. Перевірте технічні відомості, щоб дізнатися більше".

**Причина**

Не вдається завантажити звіти в UCI з помилкою "Дескриптор форми має Null-значення або не визначено". Для звітів в UCI і надалі потрібні застарілі діалогові вікна, тому в системі клієнта має бути ввімкнуто функцію *allowlegacydialogsembedding.*

**Вирішення**

1. Виберіть Параметри **>адміністрування > системних параметрів > вкладці Загальні.**

2. Установіть для параметра "Дозволити вбудовування певних застарілих діалогових вікон у клієнті браузера уніфікованого інтерфейсу" **значення Так.**
