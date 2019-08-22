---
title: Вирішення проблем із доставкою електронної пошти до пошти спільних папок
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: f7b5e5a230d26870d5e95e8762b5874f73723c6d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525165"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Вирішення проблем із доставкою електронної пошти до пошти спільних папок

Якщо зовнішніх відправників не вдається надіслати повідомлення до пошти спільних папок і відправників отримувати повідомлення про помилку: **не міг знайти (550 5.4.1)**, перевірити електронну пошту домену для спільних папок настроєно як внутрішній домен ретрансляції замість послугами авторитетний домен:

1. Відкрийте [Exchange admin центр (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Перейдіть до **потоку пошти** \> **допустимих доменів**, виберіть допустимий домен і натисніть кнопку **редагувати**.

3. У властивості сторінки цього відкриється, якщо тип домену має значення **Authoritative**, змініть значення на **внутрішньої ретрансляції** і натисніть кнопку **зберегти**.

Якщо зовнішніх відправників одержувати помилки, **ви не маєте дозволу (550 5.7.13)**, запустіть таку команду в [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) бачити дозволи для анонімних користувачів у спільній папці:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Наприклад, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Щоб дозволити зовнішнім користувачам надсилати електронну пошту до цієї спільної папки, додати CreateItems доступу права користувача Анонім. Наприклад, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
