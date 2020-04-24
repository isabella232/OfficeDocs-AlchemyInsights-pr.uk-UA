---
title: Налаштування автовідповідей для поштової скриньки
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
ms.openlocfilehash: 4ffe8d77dad7db5fd5806fe879cf4934e5ca7c4a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/23/2020
ms.locfileid: "43788903"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Налаштування автовідповідей для поштової скриньки користувача

**Спосіб 1**

1. Увійдіть на портал Microsoft 365.

2. Виберіть **Користувачів > Активні користувачі** (або **Групи > Спільні поштові скриньки**, якщо цю функцію встановлено у спільній поштовій скриньці).

3. Виберіть користувача з поштовою скринькою Microsoft Exchange.

4. У спливаючому меню праворуч перейдіть до розділу **Параметри пошти > Автовідповіді** (якщо це спільна поштова скринька, відразу клацніть **Автовідповіді**).

**Спосіб 2**

1. Увійдіть на портал адміністрування Microsoft 365, використовуючи облікові дані адміністратора.

2. Розгорніть **Центри адміністрування** та клацніть **Exchange**.

3. Клацніть зображення у верхньому правому куті, виберіть пункт**Інший користувач**, та виберіть поштову скриньку користувача, яку потрібно змінити.

4. У лівій частині виберіть **Параметри**, клацніть **Упорядкування електронної пошти**, а потім виберіть пункт **Автовідповіді.**

**Спосіб 3**

Запустіть наступний cmdlet у службі Exchange Online PowerShell:

PowerShellCopy

```
    Set-MailboxAutoReplyConfiguration
```

Докладні відомості про cmdlet див. в [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).
