---
title: Вирішення проблем із доставкою електронної пошти для спільних папок із підтримкою пошти
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
ms.openlocfilehash: ff1400f694ae037a8658356af068b4c20b8fa9d9908dafedb90db7bb6859530f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068833"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Вирішення проблем із доставкою електронної пошти для спільних папок із підтримкою пошти

Якщо зовнішні відправники не можуть надсилати повідомлення до спільних поштових папок, а відправники отримають повідомлення про помилку: не вдалося знайти **(550 5.4.1),** переконайтеся, що домен електронної пошти для спільної папки настроєно як внутрішній проміжний домен замість повноважного домену:

1. Відкрийте [Центр Exchange адміністрування (EAC).](https://docs.microsoft.com/Exchange/exchange-admin-center)

2. Перейдіть до **пункту** \> **Потік пошти допустимі** домени, виберіть допустимий домен і натисніть кнопку **Редагувати**.

3. На сторінці властивостей, що відкриється, якщо для типу домену встановлено значення Повноваження, змініть значення на Внутрішнє **реле,** а потім натисніть кнопку **Зберегти**.

Якщо зовнішні відправники отримали повідомлення про помилку, у вас немає дозволу **(550 5.7.13),** виконайте в [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) таку команду, щоб переглянути дозволи для анонімних користувачів у спільній папці:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Наприклад, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Щоб дозволити зовнішнім користувачам надсилати електронну пошту до цієї спільної папки, додайте доступ CreateItems до анонімного користувача. Наприклад, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
