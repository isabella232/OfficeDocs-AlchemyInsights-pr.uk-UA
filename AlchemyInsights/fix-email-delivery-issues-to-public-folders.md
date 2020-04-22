---
title: Вирішення проблем із доставкою електронної пошти до спільних папок із підтримкою пошти
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716373"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Вирішення проблем із доставкою електронної пошти до спільних папок із підтримкою пошти

Якщо зовнішні відправники не можуть надсилати повідомлення до спільних папок із підтримкою пошти, а відправники отримують помилку: не вдалося **знайти (550 5.4.1)**, переконайтеся, що домен електронної пошти для спільної папки настроєно як внутрішній домен ретрансляції замість основного домену:

1. Відкрийте [Центр адміністрування для Exchange](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Перейдіть до **пошти** \> **допустимі домени**, виберіть допустимий домен і натисніть кнопку **змінити**.

3. На сторінці властивостей, що відкриється, якщо тип домену встановлено **авторитетне**, змініть значення на **внутрішній ретранслятор** і натисніть кнопку **зберегти**.

Якщо зовнішні відправники отримують помилку, у **вас немає дозволу (550 5.7.13)**, виконайте таку команду в [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) , щоб переглянути дозволи для анонімних користувачів у спільних папок:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Наприклад, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Щоб дозволити зовнішнім користувачам надсилати повідомлення електронної пошти до цієї спільної папки, додайте права доступу до CreateItems, щоб користувач анонімний. Наприклад, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
