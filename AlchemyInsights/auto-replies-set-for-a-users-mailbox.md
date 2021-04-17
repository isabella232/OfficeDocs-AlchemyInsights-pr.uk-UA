---
title: Налаштування автовідповідей для поштової скриньки
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 60af581e7fe508ab9644a53873bcd551b3aacff1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820955"
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

3. Клацніть зображення у верхньому правому куті, виберіть пункт **Інший користувач**, та виберіть поштову скриньку користувача, яку потрібно змінити.

4. У лівій частині виберіть **Параметри**, клацніть **Упорядкування електронної пошти**, а потім виберіть пункт **Автовідповіді.**

**Спосіб 3**

Запустіть наступний cmdlet у службі Exchange Online PowerShell:

PowerShellCopy

```
    Set-MailboxAutoReplyConfiguration
```

Докладні відомості про cmdlet див. в [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).
