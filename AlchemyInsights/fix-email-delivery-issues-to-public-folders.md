---
title: Вирішення проблем із доставкою електронної пошти до спільних папок із підтримкою пошти
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
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: da35ae4bd911fb75f23cc1c99aacbaa2392425dd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677949"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Вирішення проблем із доставкою електронної пошти до спільних папок із підтримкою пошти

Якщо зовнішні відправники не можуть надсилати повідомлення до спільних папок із підтримкою пошти, а відправники отримують повідомлення про помилку: **не вдалося знайти (550 5.4.1)**, переконайтеся, що домен електронної пошти для спільної папки настроєно як внутрішній домен ретрансляції, а не важливий домен:

1. Відкрийте [Центр адміністрування Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Перейдіть на **Mail flow** сторінку \> **допустимі домени**передавання пошти, виберіть допустимий домен і натисніть кнопку **редагувати**.

3. На сторінці властивостей, що Відкриється, якщо тип домену має значення " **авторитетний**", змініть значення на **внутрішній ретранслятор** і натисніть кнопку " **зберегти**".

Якщо зовнішні відправники отримують повідомлення про помилку, у **якому немає дозволу (550 5.7.13)**, виконайте таку команду в [службі Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) , щоб переглянути дозволи для анонімних користувачів у спільній папці.

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Наприклад, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Щоб дозволити зовнішнім користувачам надсилати повідомлення електронної пошти до цієї загальнодоступної папки, додайте до анонімного користувача доступ до списку CreateItems. Наприклад, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
