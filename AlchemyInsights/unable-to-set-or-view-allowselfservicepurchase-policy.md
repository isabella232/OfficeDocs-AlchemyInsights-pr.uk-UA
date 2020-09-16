---
title: Не вдається встановити або переглянути політику AllowSelfServicePurchase
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
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735220"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Не вдається встановити або переглянути політику AllowSelfServicePurchase

Під час спроби встановити або переглянути політику AllowSelfServicePurchase з'являється таке повідомлення про помилку:

*HandleError: не вдалося отримати політику продукту з ідентифікатором політик "AllowSelfServicePurchase", Erritmessage-вихідне підключення було закрито: сталася неочікувана помилка на сторінці "надсилати".*

Це може бути пов'язано зі старою версією захисту транспортного шару (TLS). Щоб підключитися до служби MSCommerce, потрібно використовувати протокол TLS 1,2 або новішої версії.  

Виконайте наведені нижче дії, щоб увімкнути або настроїти протокол TLS для 1,2, перевірка та повторіть спробу.
 1. У командному рядку PowerShell (PS C: \) Укажіть таку команду, щоб установити протокол TLS для версії 1,2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Перевірте протокол TLS (-ів) у програмі, використовуючи таку команду:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Повторіть команду "отримати або оновити" за потреби.

