---
title: Не вдається встановити або переглянути політику AllowSelfServicePurchase
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
- "9001212"
- "3526"
ms.openlocfilehash: 255dbe35b808b3fe6b5707779251bf3f4a7e1c269c8b6f0ac2cb43ca03c469e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020213"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Не вдається встановити або переглянути політику AllowSelfServicePurchase

Під час спроби встановити або переглянути політику AllowSelfServicePurchase з'являється таке повідомлення про помилку:

*HandleError: не вдалося отримати політику продукту за допомогою PolicyId "AllowSelfServicePurchase", ErrorMessage – основне підключення закрито: під час надсилання сталася неочікувана помилка.*

Причиною цього може бути старіша версія протоколу TLS. Щоб підключити службу MSCommerce, потрібно використовувати TLS 1.2 або більше.  

Щоб увімкнути або встановити протокол TLS 1.2, перевірити та повторити спробу, виконайте наведені нижче дії.
 1. У командному рядку PowerShell (PS C: введіть таку команду, щоб установити протокол \) TLS версії 1.2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Перевірте використовувані протоколи TLS за допомогою такої команди:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. За потреби повторіть ці команди: Отримати або Оновити.

