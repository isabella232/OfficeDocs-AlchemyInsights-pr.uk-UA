---
title: Не вдається встановити або переглянути Дозволяєпослугуправила політики
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158582"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Не вдається встановити або переглянути Дозволяєпослугуправила політики

Під час спроби встановити або переглянути Дозволяєполітики, з'являється таке повідомлення про помилку:

*HandleError: не вдалося отримати політику продукту з політикою політики "Дозволяєповідомлення", помилка-базове підключення закрито: сталася неочікувана помилка під час надсилання.*

Це може бути через стару версію транспортний рівень безпеки (TLS). Щоб підключити службу MSCommerce, потрібно використовувати TLS 1,2 або більше.  

Виконайте наведені нижче дії, щоб увімкнути/встановити протокол TLS 1,2, перевірте і повторіть спробу.
 1. У командному рядку PowerShell (PS C:\) введіть таку команду, щоб УСТАНОВИТИ протокол TLS версії 1,2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Перевірте, чи протокол TLS використовується, за допомогою такої команди:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Повторіть спробу отримати або оновити команди, за потреби.

