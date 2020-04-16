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
ms.openlocfilehash: aeeb2e1e76fe602d2767b422797452fd1155fdd5
ms.sourcegitcommit: fdfd41c2bfb2d45003b3906e6469377384a91cb5
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2020
ms.locfileid: "43509538"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Налаштування автовідповідей для поштової скриньки користувача

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

```
    Set-MailboxAutoReplyConfiguration
```

Докладні відомості про cmdlet див. в [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).
