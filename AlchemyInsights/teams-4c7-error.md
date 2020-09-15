---
title: Помилка 4C7 для команд
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
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700224"
---
# <a name="4c7-error-in-microsoft-teams"></a>Помилка 4C7 в командах Microsoft

Ця помилка виникає через те, що команди Microsoft потребують автентифікації форм. Якщо розгорнути служби Федерації Active Directory (AD FS), автентифікація форм не активовано для інтрамережі за замовчуванням. Якщо Windows інтегровану автентифікацію не вдасться, з'явиться запит на вхід за допомогою автентифікації форм.

Щоб вирішити цю проблему, увімкніть автентифікацію форм за допомогою оснастки консолі керування РЕКЛАМНИМИ FS Microsoft (MMC) на комп'ютері, на якому використовується Локальна копія Active Directory. Щоб зробити це, виконайте такі дії. 

1. В області переходів перейдіть до **політики автентифікації**.
2. У розділі **дії** в області відомостей виберіть пункт **редагування глобальної основної автентифікації**.
3. На вкладці **інтрамережа** натисніть кнопку **автентифікація форми**.
4. Натисніть **кнопку OK** (або **Додати**).