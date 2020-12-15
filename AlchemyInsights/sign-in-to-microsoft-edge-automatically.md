---
title: Автоматичне входу в Microsoft EDGE
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678820"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Автоматичне входу в Microsoft EDGE

Microsoft EDGE використовує обліковий запис ОС за замовчуванням, щоб автоматично ввійти в користувача відповідно до способу настроювання пристрою користувача. 

Нижче описано сценарії кожного типу конфігурації пристрою та його залежного процесу для реєстрації користувачів:

1. **Пристрій Hybrid/AAD-J**: цей параметр доступний у Windows 10, на рівні вікна та відповідні версії сервера. Користувачі автоматично мають доступ до своїх облікових записів "Azure Active Directory (AD)".
2. **Пристрій входить до складу домену**: цей параметр доступний у Windows 10, на рівні вікна, і відповідні версії сервера. За замовчуванням користувачі з обліковими записами доменів не мають автоматичного входу; Щоб увімкнути функцію автоматичного входу, скористайтеся політикою **ConfigureOnPremisesAccountAutoSignIn** . Щоб увімкнути автоматичний вхід для користувачів із обліковими записами Azure AD, спробуйте гібридне приєднання до своїх пристроїв.
3. Обліковий **запис за замовчуванням операційної системи – це обліковий запис Microsoft**: цей параметр доступний у Windows 10 RS3 (версія 1709, збірка 10.0.16299) і пізніші версії. На корпоративних пристроях навряд чи виникне ситуація. Однак, якщо обліковий запис за замовчуванням для ОС – це обліковий запис Microsoft, Microsoft EDGE автоматично ввійде в користувача за допомогою облікового запису Microsoft.
 
 
