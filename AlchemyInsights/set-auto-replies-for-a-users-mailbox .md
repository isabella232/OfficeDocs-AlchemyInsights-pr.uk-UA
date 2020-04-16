---
title: Установлення автовідповідей для поштової скриньки користувача
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: e3cc01298c10fd3ba21327a7fb5cc5396d0ad74d
ms.sourcegitcommit: 23e5b94f1758bfe202008384e300b81816975375
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/14/2020
ms.locfileid: "43506653"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Установлення автовідповідей для поштової скриньки користувача

**Спосіб 1**

1. Увійдіть на портал Office 365.

2. Виберіть **Користувачів > Активні користувачі** (або **Групи > Спільні поштові скриньки**, якщо цю функцію встановлено у спільній поштовій скриньці).

3. Виберіть користувача з поштовою скринькою Microsoft Exchange.

4. У спливаючому меню праворуч перейдіть до розділу **Параметри пошти > Автовідповіді** (якщо це спільна поштова скринька, відразу клацніть **Автовідповіді**).

**Спосіб 2**

1. Увійдіть на портал адміністрування Office 365, використовуючи облікові дані адміністратора.

2. Розгорніть **Центри адміністрування** та клацніть **Exchange**.

3. Клацніть зображення у верхньому правому куті, виберіть пункт**Інший користувач**, та виберіть поштову скриньку користувача, яку потрібно змінити.

4. У лівій частині виберіть **Параметри**, клацніть **Упорядкування електронної пошти**, а потім виберіть пункт **Автовідповіді.**

**Спосіб 3**

Запустіть наступний cmdlet у службі Exchange Online PowerShell:

PowerShellCopy

    Set-MailboxAutoReplyConfiguration

Докладні відомості про cmdlet див. в [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).
