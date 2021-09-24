---
title: Повернення від DNS-серверів Microsoft до керування власними записами DNS
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13988"
- "14"
ms.openlocfilehash: a228bcda1220011ab994de7aa70f19ea092e2142
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506977"
---
# <a name="changing-from-microsoft-nameservers-back-to-managing-your-own-dns-records"></a>Повернення від DNS-серверів Microsoft до керування власними записами DNS

Ви раніше змінили записи DNS-серверів, щоб вони вказували на microsoft (ns1.bdm.microsoftonline.com), але тепер вирішили керувати власними записами DNS:

На веб-сайті реєстратора доменів поверніть реєстратора імен до попереднього або попереднього параметра. Якщо ви не знайомі з DNS, зверніться до служби підтримки на веб-сайті реєстратора доменів. Зверніть увагу, що розгортання змін на серверах імен може зайняти до 48 годин. 

1. На порталі Microsoft 365 адміністрування перейдіть до розділу **Настройки** Domains (Домени) , установіть прапорець поруч із потрібним доменом і виберіть елемент Manage DNS (Керувати  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains) **службою DNS).** 

2. У майстрі виберіть **пункт Додати власні записи DNS** і виконайте роботу майстра. Зміниться спосіб керування записами DNS, а потім дає змогу додати настроювані записи DNS, необхідні для підтримки вибраних служб.

Крім того, якщо ви змінили записи DNS-сервера до корпорації Майкрософт і маєте веб-сайт, можна додати записи DNS для веб-сайту, щоб не повертати сервери імен. Докладні відомості див. в розділі Оновлення записів DNS для збереження [веб-сайту в поточного постачальника послуг розміщення.](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)


